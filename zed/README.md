# Ember One for Zed

Zed theme-family JSON files can contain multiple variants. This port contains
both `Ember One Dark` and `Ember One Light`.

## Install

From the root of this repository on macOS or Linux:

```sh
mkdir -p "${XDG_CONFIG_HOME:-$HOME/.config}/zed/themes"
cp zed/ember-one.json \
  "${XDG_CONFIG_HOME:-$HOME/.config}/zed/themes/ember-one.json"
```

On Windows, copy it to `%USERPROFILE%\AppData\Roaming\Zed\themes\`.

Restart Zed if the themes do not appear immediately. Open the Theme Selector
with `Cmd+K Cmd+T` on macOS or `Ctrl+K Ctrl+T` on Linux and Windows, or set the
theme in `settings.json`:

```json
{
  "theme": {
    "mode": "system",
    "dark": "Ember One Dark",
    "light": "Ember One Light"
  }
}
```

See Zed's [official theme documentation][themes] for local-theme paths and
selection options.

[themes]: https://zed.dev/docs/themes#local-themes
