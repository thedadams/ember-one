# Ember One for Neovim

The single colorscheme file selects its light or dark palette from Neovim's
`background` option.

## Install

From the root of this repository on macOS or Linux:

```sh
mkdir -p "${XDG_CONFIG_HOME:-$HOME/.config}/nvim/colors"
cp nvim/ember-one.lua \
  "${XDG_CONFIG_HOME:-$HOME/.config}/nvim/colors/ember-one.lua"
```

Load it for the current session with `:colorscheme ember-one`, or add this to
`init.lua` to make it permanent:

```lua
vim.o.background = "light" -- or "dark"
vim.cmd.colorscheme("ember-one")
```

Neovim searches its runtime path for `colors/ember-one.lua`. See the
[official `:colorscheme` documentation][colorscheme] for lookup behavior.

[colorscheme]: https://neovim.io/doc/user/syntax.html#%3Acolorscheme
