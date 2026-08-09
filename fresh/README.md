# Ember One for Fresh

Fresh loads one theme per JSON file, so this port provides separate dark and
light files.

## Install

From the root of this repository on macOS or Linux:

```sh
mkdir -p "${XDG_CONFIG_HOME:-$HOME/.config}/fresh/themes"
cp fresh/ember-one-dark.json fresh/ember-one-light.json \
  "${XDG_CONFIG_HOME:-$HOME/.config}/fresh/themes/"
```

Open the command palette with `Ctrl+P`, choose **Select Theme**, and select
`ember-one-dark` or `ember-one-light`.

Alternatively, set the theme directly in Fresh's config file (normally
`~/.config/fresh/config.json`):

```json
{
  "theme": "ember-one-dark.json"
}
```

The filename is resolved relative to Fresh's `themes` directory. See the
[official Fresh theme documentation][themes] for the theme selector, config
syntax, and other supported theme locations.

[themes]: https://getfresh.dev/docs/features/themes
