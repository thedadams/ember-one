# Ember One for Zellij

Zellij allows multiple named themes in one KDL `themes` block. This port
contains `ember-one-dark` and `ember-one-light`.

## Install

Run `zellij setup --check` to confirm the active configuration directory. With
the usual XDG location, install the theme from the root of this repository:

```sh
mkdir -p "${XDG_CONFIG_HOME:-$HOME/.config}/zellij/themes"
cp zellij/ember-one.kdl \
  "${XDG_CONFIG_HOME:-$HOME/.config}/zellij/themes/ember-one.kdl"
```

If `zellij setup --check` reports another configuration directory, use its
`themes/` subdirectory instead. Select a variant in `config.kdl`:

```kdl
theme "ember-one-dark"
```

Use `theme "ember-one-light"` for the light variant. You can also select a
theme for one launch with `zellij options --theme ember-one-dark`.

See Zellij's [official theme documentation][themes] for theme locations and
selection behavior.

[themes]: https://zellij.dev/documentation/themes.html
