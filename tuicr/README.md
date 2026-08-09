# Ember One for tuicr

tuicr uses one flat TOML palette and one TextMate syntax theme per variant.

## Install

From the root of this repository on macOS or Linux:

```sh
mkdir -p "${XDG_CONFIG_HOME:-$HOME/.config}/tuicr/themes"
cp tuicr/ember-one-dark.toml tuicr/ember-one-dark-syntax.tmTheme \
  tuicr/ember-one-light.toml tuicr/ember-one-light-syntax.tmTheme \
  "${XDG_CONFIG_HOME:-$HOME/.config}/tuicr/themes/"
```

In `$XDG_CONFIG_HOME/tuicr/config.toml` (normally
`~/.config/tuicr/config.toml`), remove any top-level `theme` setting and
configure automatic pairing:

```toml
appearance = "system"
theme_dark = "ember-one-dark"
theme_light = "ember-one-light"
```

An explicit `theme` setting takes precedence over the paired variants. To test
one variant without changing the configuration, run:

```sh
tuicr --theme ember-one-dark
```

On Windows, install the four files in `%APPDATA%\tuicr\themes\` and edit
`%APPDATA%\tuicr\config.toml`. See tuicr's [official configuration
documentation][config] for lookup and precedence details.

[config]: https://github.com/agavra/tuicr/blob/main/docs/CONFIG.md#themes
