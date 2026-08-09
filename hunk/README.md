# Ember One for Hunk

Hunk stores custom themes in its configuration rather than a separate theme
directory. These files are complete configurations containing `theme =
"custom"` and an Ember One `[custom_theme]` table.

## Install

If you do not already have a Hunk configuration, copy the variant you want:

```sh
mkdir -p "${XDG_CONFIG_HOME:-$HOME/.config}/hunk"
cp hunk/ember-one-dark.toml \
  "${XDG_CONFIG_HOME:-$HOME/.config}/hunk/config.toml"
```

Use `hunk/ember-one-light.toml` instead for the light variant.

If `config.toml` already exists, do not replace it. Merge the `theme =
"custom"` setting and the `[custom_theme]` tables from the chosen file into the
existing configuration. The same configuration can be scoped to one repository
by saving it as `.hunk/config.toml` there.

See Hunk's [official theme documentation][themes] for custom-theme tables,
named themes, and configuration precedence.

[themes]: https://github.com/modem-dev/hunk/blob/main/docs/themes.md
