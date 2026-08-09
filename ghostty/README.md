# Ember One for Ghostty

Ghostty uses one palette per theme file and pairs variants from its main
configuration.

## Install

From the root of this repository on macOS or Linux:

```sh
mkdir -p "${XDG_CONFIG_HOME:-$HOME/.config}/ghostty/themes"
cp ghostty/ember-one-dark ghostty/ember-one-light \
  "${XDG_CONFIG_HOME:-$HOME/.config}/ghostty/themes/"
```

Add this line to `$XDG_CONFIG_HOME/ghostty/config` (normally
`~/.config/ghostty/config`):

```ini
theme = dark:ember-one-dark,light:ember-one-light
```

Ghostty will follow the system appearance and select the matching variant. It
reloads the configuration after the file is saved; the themes can also be
checked with `ghostty +list-themes`.

See Ghostty's [official color-theme documentation][themes] for theme lookup
paths and light/dark pairing.

[themes]: https://ghostty.org/docs/features/theme
