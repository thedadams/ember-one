# Ember One

Ember One is a personal color scheme collected in one place. This repository is
the home for its palette, theme configurations, installation notes, and visual
references.

The repository follows the organization of [Flexoki][flexoki]: each supported
app or tool gets a top-level directory, while shared project assets live in
underscore-prefixed directories.

## Themes

| App or tool | Variants | Directory |
| --- | --- | --- |
| Fresh | Dark and light | [`fresh/`](fresh/) |
| Ghostty | Dark and light | [`ghostty/`](ghostty/) |
| Hunk | Dark and light | [`hunk/`](hunk/) |
| Neovim | Dark and light, adaptive | [`nvim/`](nvim/) |
| rootshell | Dark | [`rootshell/`](rootshell/) |
| Slack | Custom | [`slack/`](slack/) |
| Telegram | Dark and light, cloud | [`telegram/`](telegram/) |
| Terminal.app | Dark and light | [`terminal/`](terminal/) |
| tuicr | Dark and light | [`tuicr/`](tuicr/) |
| Zed | Dark and light, combined | [`zed/`](zed/) |
| Zellij | Dark and light, combined | [`zellij/`](zellij/) |

## Repository layout

```text
ember-one/
├── _generators/   # Scripts or templates that produce theme files
├── _images/       # Screenshots and project artwork
├── _samples/      # Reference files used to check syntax colors
├── app-name/      # Theme files and app-specific installation notes
├── LICENSE
└── README.md
```

Theme ports belong at the repository root and should use the lowercase name of
their target app or tool, such as `alacritty/`, `vscode/`, or `zed/`.

## Adding a theme

1. Create a top-level directory named after the target app or tool.
2. Add separate light and dark files when the app supports both variants.
3. Name distributable themes `Ember One Light` and `Ember One Dark`.
4. Include an app-specific `README.md` with installation instructions and any
   compatibility notes.
5. Add useful screenshots to `_images/` and reusable syntax fixtures to
   `_samples/`.
6. Add the new port to the themes table above.

Generated output should be committed so that users can install a theme without
running a build step. Keep its source template or generator in `_generators/`.

## License

[MIT](LICENSE) © 2026 Donnie Adams

[flexoki]: https://github.com/kepano/flexoki
