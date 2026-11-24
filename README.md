# Blue (Vim Port)

A port of Vim’s classic **“blue.vim”** colorscheme for Visual Studio Code: a deep blue background with gold text, white statements and cyan constants.

------

## 🎨 About the Theme

`blue.vim` was written by **Steven Vertigan** and ships with Vim. It uses a dark blue background (`#000087`) with gold text (`#ffd700`), grey bold comments, white keywords, orange bold types and cyan constants. This port keeps the colors of the GUI version (`guifg`/`guibg`) and maps Vim’s highlight groups to TextMate scopes and VS Code UI colors.

### ✳️ Highlights

| Group         | Color (hex)            | Description                    |
| ------------- | ---------------------- | ------------------------------ |
| **Normal**    | `#ffd700` on `#000087` | Gold on deep blue              |
| **Comment**   | `#878787`              | Grey, bold                     |
| **Constant**  | `#5fffff`              | Cyan (strings, numbers)        |
| **Statement** | `#ffffff`              | White                          |
| **PreProc**   | `#00ff00`              | Green                          |
| **Type**      | `#ffa500`              | Orange, bold                   |
| **Special**   | `#d787d7`              | Pink                           |
| **Function**  | `#bcbcbc`              | Light grey (links to `Identifier`) |

------

## 🎭 Variants

| Theme                         | Description                                  |
| ----------------------------- | -------------------------------------------- |
| **Blue (Vim Port)**           | The port, with bold comments and types       |
| **Blue (Vim Port, no bold)**  | Same colors, without bold text               |

The sidebar and panel (`#000075`) are a shade darker than the editor, because Blue itself only knows one background. Activity bar, title bar and status bar share Vim’s `TitleBar` look (`#1f4f87` with gold text). Tabs, menus, widgets and list selection stay within the blue family (`#0f3f77`, `#1f4f87`, `#005faf`); the active tab matches the editor background with a cyan top border.

Not 1:1:
- Vim’s `Visual` is white on `#008787`. That teal is used only for the editor selection; VS Code cannot switch the text color of a selection, so it keeps the syntax colors.
- Vim’s `Search` and `MatchParen` are reversed colors. VS Code cannot invert text, so matches get a gold background, and a matching bracket gets a gold border.
- Diff backgrounds are solid as in Vim: `#5f875f` for added and `#af5faf` for removed text. Changed text has no extra background; `#5f87af` is only used for the modified marker in the gutter and the diagonal fill.

------

## 🧩 Installation

Works with **Visual Studio Code** and **VSCodium**. Search for **Blue (Vim Port)** by **r11s** in the Extensions view, or open the page directly:

- VS Code: [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=r11s.blue-vscode-theme)
- VSCodium: [Open VSX](https://open-vsx.org/extension/r11s/blue-vscode-theme)

Or install a local `.vsix` via **Extensions: Install from VSIX…**. Then select the theme under **Preferences: Color Theme**.

------

## ⚙️ Recommended Settings

```jsonc
{
  "editor.semanticHighlighting.enabled": true,
  "editor.bracketPairColorization.enabled": false,
  "editor.guides.bracketPairs": false,
  "editor.renderWhitespace": "none",
  "editor.cursorBlinking": "solid"
}
```

------

## ⚖️ License

Released under the [Vim License](https://github.com/vim/vim/blob/master/runtime/doc/uganda.txt).

This theme is a **port** of **“blue.vim”** (original author and maintainer: **Steven Vertigan** <steven@vertigan.wattle.id.au>; current version in the Vim colorschemes, https://github.com/vim/colorschemes, Last Change 2026 Oct 02). It is not the original. All modifications and adaptations are provided under the same terms as Vim itself. See `LICENSE`.

------

## 🛠 Maintainers

- **Ported by:** Rainer Strauss ([r11s](https://github.com/r11s))
- **Original blue.vim author:** Steven Vertigan
- **Vim Project:** https://www.vim.org
