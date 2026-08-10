# Ember One

Ember One is a dark, charcoal-first color scheme for code, terminals, and
productivity tools. It pairs a warm ember-orange with crisp cyan and blue, then
rounds out the palette with vivid—but never neon—supporting colors.

The `500` value of each accent is the canonical Ember One color. The remaining
values extend that color from pale `50` through deep `950` shades.

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

## Standard palette

| Role | Name | Hex | RGB |
| --- | --- | --- | --- |
| Deep / inactive | `black` | `#191D24` | `25, 29, 36` |
| Main background | `bg` | `#20242C` | `32, 36, 44` |
| Panels | `bg-2` | `#282E37` | `40, 46, 55` |
| Raised UI | `ui` | `#303743` | `48, 55, 67` |
| Hover / border | `ui-2` | `#37404D` | `55, 64, 77` |
| Selection / active | `ui-3` | `#3F4F66` | `63, 79, 102` |
| Strong border | `border` | `#434D5B` | `67, 77, 91` |
| Faint text | `tx-3` | `#7F8998` | `127, 137, 152` |
| Muted text | `tx-2` | `#AAB4C0` | `170, 180, 192` |
| Primary text | `tx` | `#E1E6EC` | `225, 230, 236` |
| Strong text | `paper` | `#F5F7FA` | `245, 247, 250` |

| Accent | Name | Hex | Typical roles |
| --- | --- | --- | --- |
| Red | `red-500` | `#EA5670` | Errors, destructive actions, keywords |
| Orange | `orange-500` | `#F58B45` | Brand accent, numbers, ember highlight |
| Yellow | `yellow-500` | `#DDBB52` | Warnings, attention, modified state |
| Green | `green-500` | `#99C45C` | Success, strings, additions |
| Cyan | `cyan-500` | `#36CDBB` | Functions, high-signal information |
| Blue | `blue-500` | `#5FAAF7` | Links, focus, selection, primary actions |
| Purple | `purple-500` | `#B96EF2` | Types, special syntax |
| Magenta | `magenta-500` | `#E655A7` | Constants, tags, decorators |

## Base

| Name | Hex | RGB |
| --- | --- | --- |
| `paper` | `#F5F7FA` | `245, 247, 250` |
| `base-50` | `#E1E6EC` | `225, 230, 236` |
| `base-100` | `#C9D1D9` | `201, 209, 217` |
| `base-150` | `#AAB4C0` | `170, 180, 192` |
| `base-200` | `#9CA7B3` | `156, 167, 179` |
| `base-300` | `#8792A0` | `135, 146, 160` |
| `base-400` | `#7F8998` | `127, 137, 152` |
| `base-500` | `#788391` | `120, 131, 145` |
| `base-600` | `#667180` | `102, 113, 128` |
| `base-700` | `#56606E` | `86, 96, 110` |
| `base-800` | `#434D5B` | `67, 77, 91` |
| `base-850` | `#3F4F66` | `63, 79, 102` |
| `base-900` | `#37404D` | `55, 64, 77` |
| `base-950` | `#303743` | `48, 55, 67` |
| `bg-2` | `#282E37` | `40, 46, 55` |
| `bg` | `#20242C` | `32, 36, 44` |
| `black` | `#191D24` | `25, 29, 36` |

## Red

| Name | Hex | RGB |
| --- | --- | --- |
| `red-50` | `#F7E8EC` | `247, 232, 236` |
| `red-100` | `#F8D9DD` | `248, 217, 221` |
| `red-150` | `#F8C9CF` | `248, 201, 207` |
| `red-200` | `#F8BAC1` | `248, 186, 193` |
| `red-300` | `#F6A3AC` | `246, 163, 172` |
| `red-400` | `#F28391` | `242, 131, 145` |
| **`red-500`** | **`#EA5670`** | **`234, 86, 112`** |
| `red-600` | `#C84F64` | `200, 79, 100` |
| `red-700` | `#A74758` | `167, 71, 88` |
| `red-800` | `#863F4D` | `134, 63, 77` |
| `red-850` | `#723A45` | `114, 58, 69` |
| `red-900` | `#5D343E` | `93, 52, 62` |
| `red-950` | `#432C34` | `67, 44, 52` |

## Orange

| Name | Hex | RGB |
| --- | --- | --- |
| `orange-50` | `#F7EDE9` | `247, 237, 233` |
| `orange-100` | `#F8E2D8` | `248, 226, 216` |
| `orange-150` | `#F8D8C7` | `248, 216, 199` |
| `orange-200` | `#F9CDB6` | `249, 205, 182` |
| `orange-300` | `#F9BD9C` | `249, 189, 156` |
| `orange-400` | `#F8A878` | `248, 168, 120` |
| **`orange-500`** | **`#F58B45`** | **`245, 139, 69`** |
| `orange-600` | `#D07A43` | `208, 122, 67` |
| `orange-700` | `#AD6940` | `173, 105, 64` |
| `orange-800` | `#8B583C` | `139, 88, 60` |
| `orange-850` | `#744D39` | `116, 77, 57` |
| `orange-900` | `#5F4235` | `95, 66, 53` |
| `orange-950` | `#44342F` | `68, 52, 47` |

## Yellow

| Name | Hex | RGB |
| --- | --- | --- |
| `yellow-50` | `#F3F1EB` | `243, 241, 235` |
| `yellow-100` | `#F0EBDB` | `240, 235, 219` |
| `yellow-150` | `#EEE6CC` | `238, 230, 204` |
| `yellow-200` | `#EBE0BC` | `235, 224, 188` |
| `yellow-300` | `#E8D7A4` | `232, 215, 164` |
| `yellow-400` | `#E3CB82` | `227, 203, 130` |
| **`yellow-500`** | **`#DDBB52`** | **`221, 187, 82`** |
| `yellow-600` | `#BCA14E` | `188, 161, 78` |
| `yellow-700` | `#9C8849` | `156, 136, 73` |
| `yellow-800` | `#7D6F43` | `125, 111, 67` |
| `yellow-850` | `#695F3E` | `105, 95, 62` |
| `yellow-900` | `#565039` | `86, 80, 57` |
| `yellow-950` | `#3E3C32` | `62, 60, 50` |

## Green

| Name | Hex | RGB |
| --- | --- | --- |
| `green-50` | `#ECF2EB` | `236, 242, 235` |
| `green-100` | `#E2EDDC` | `226, 237, 220` |
| `green-150` | `#D9E8CD` | `217, 232, 205` |
| `green-200` | `#CFE3BE` | `207, 227, 190` |
| `green-300` | `#C2DCA7` | `194, 220, 167` |
| `green-400` | `#AFD187` | `175, 209, 135` |
| **`green-500`** | **`#99C45C`** | **`153, 196, 92`** |
| `green-600` | `#84A855` | `132, 168, 85` |
| `green-700` | `#6F8D4E` | `111, 141, 78` |
| `green-800` | `#5B7346` | `91, 115, 70` |
| `green-850` | `#4E6341` | `78, 99, 65` |
| `green-900` | `#41523B` | `65, 82, 59` |
| `green-950` | `#323E33` | `50, 62, 51` |

## Cyan

| Name | Hex | RGB |
| --- | --- | --- |
| `cyan-50` | `#E6F3F4` | `230, 243, 244` |
| `cyan-100` | `#D6EFED` | `214, 239, 237` |
| `cyan-150` | `#C7EBE7` | `199, 235, 231` |
| `cyan-200` | `#B7E7E0` | `183, 231, 224` |
| `cyan-300` | `#9DE1D7` | `157, 225, 215` |
| `cyan-400` | `#78D8CA` | `120, 216, 202` |
| **`cyan-500`** | **`#36CDBB`** | **`54, 205, 187`** |
| `cyan-600` | `#37B0A2` | `55, 176, 162` |
| `cyan-700` | `#35938A` | `53, 147, 138` |
| `cyan-800` | `#327872` | `50, 120, 114` |
| `cyan-850` | `#2F6663` | `47, 102, 99` |
| `cyan-900` | `#2B5554` | `43, 85, 84` |
| `cyan-950` | `#253F42` | `37, 63, 66` |

## Blue

| Name | Hex | RGB |
| --- | --- | --- |
| `blue-50` | `#E6F0FA` | `230, 240, 250` |
| `blue-100` | `#D8E8FB` | `216, 232, 251` |
| `blue-150` | `#C9E1FB` | `201, 225, 251` |
| `blue-200` | `#BBD9FB` | `187, 217, 251` |
| `blue-300` | `#A5CEFA` | `165, 206, 250` |
| `blue-400` | `#87BEF9` | `135, 190, 249` |
| **`blue-500`** | **`#5FAAF7`** | **`95, 170, 247`** |
| `blue-600` | `#5493D4` | `84, 147, 212` |
| `blue-700` | `#4A7CB1` | `74, 124, 177` |
| `blue-800` | `#3F6690` | `63, 102, 144` |
| `blue-850` | `#38587B` | `56, 88, 123` |
| `blue-900` | `#314A66` | `49, 74, 102` |
| `blue-950` | `#28394D` | `40, 57, 77` |

## Purple

| Name | Hex | RGB |
| --- | --- | --- |
| `purple-50` | `#EFEAFA` | `239, 234, 250` |
| `purple-100` | `#E9DDFA` | `233, 221, 250` |
| `purple-150` | `#E3D0FA` | `227, 208, 250` |
| `purple-200` | `#DDC2FA` | `221, 194, 250` |
| `purple-300` | `#D4AEF8` | `212, 174, 248` |
| `purple-400` | `#C893F6` | `200, 147, 246` |
| **`purple-500`** | **`#B96EF2`** | **`185, 110, 242`** |
| `purple-600` | `#9F62D0` | `159, 98, 208` |
| `purple-700` | `#8555AE` | `133, 85, 174` |
| `purple-800` | `#6C498E` | `108, 73, 142` |
| `purple-850` | `#5C4179` | `92, 65, 121` |
| `purple-900` | `#4C3965` | `76, 57, 101` |
| `purple-950` | `#382F4C` | `56, 47, 76` |

## Magenta

| Name | Hex | RGB |
| --- | --- | --- |
| `magenta-50` | `#F6E8F2` | `246, 232, 242` |
| `magenta-100` | `#F7D9E9` | `247, 217, 233` |
| `magenta-150` | `#F6C9E1` | `246, 201, 225` |
| `magenta-200` | `#F6BAD8` | `246, 186, 216` |
| `magenta-300` | `#F3A2CC` | `243, 162, 204` |
| `magenta-400` | `#EF82BB` | `239, 130, 187` |
| **`magenta-500`** | **`#E655A7`** | **`230, 85, 167`** |
| `magenta-600` | `#C44E91` | `196, 78, 145` |
| `magenta-700` | `#A4467C` | `164, 70, 124` |
| `magenta-800` | `#843E68` | `132, 62, 104` |
| `magenta-850` | `#70395B` | `112, 57, 91` |
| `magenta-900` | `#5C334E` | `92, 51, 78` |
| `magenta-950` | `#432B3E` | `67, 43, 62` |

## Usage guidance

- Use `500` accents for syntax and high-contrast elements on Ember One's dark
  backgrounds.
- Use `400` accents for brighter hover or emphasized states.
- Use `600`–`800` accents for borders, pressed states, and tinted surfaces.
- Use `50`–`300` accents primarily for light-mode surfaces, subtle fills, or
  text on deep accent backgrounds.
- Keep large surfaces charcoal. Accent colors work best as signals rather than
  full-screen backgrounds.

## Design notes

- **Foundation:** Cool charcoal with a slight blue cast; never pure black.
- **Temperature:** Warm-leaning overall, led by orange and balanced by cyan and
  blue.
- **Saturation:** Vivid and clear, but softened enough for long work sessions.
- **Contrast:** Bright primary text and restrained secondary text preserve
  hierarchy without washing out the accents.

Ember One was created by Donnie Adams.

## License

[MIT](LICENSE) © 2026 Donnie Adams

[flexoki]: https://github.com/kepano/flexoki
