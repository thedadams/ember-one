# Ember One for Flow

Flow loads custom themes from its configuration directory. This port provides
separate dark and light JSON themes with Tree-sitter syntax colors.

## Install

From the root of this repository on macOS or Linux:

```sh
mkdir -p "${XDG_CONFIG_HOME:-$HOME/.config}/flow/themes"
cp "flow/Ember One Dark.json" "flow/Ember One Light.json" \
  "${XDG_CONFIG_HOME:-$HOME/.config}/flow/themes/"
```

Set the dark and light variants in
`${XDG_CONFIG_HOME:-$HOME/.config}/flow/config`:

```text
theme "Ember One Dark"
light_theme "Ember One Light"
```

Flow follows the active appearance; pass `flow --dark` or `flow --light` to
force a variant. Restart Flow after installing the files if the themes do not
appear immediately.
