# Sublime Text 4 Theme

Sublime Text 4 Dark theme for [Zed](https://zed.dev), generated from the [Vine](https://github.com/dallasgere/vine) VS Code theme.

## Install locally

1. In Zed, open the command palette and run `zed: install dev extension`.
2. Select this folder.
3. Run `theme selector: toggle` and pick `Sublime Text 4 Dark`.

Or copy the files in `themes/` into `~/.config/zed/themes/`.

## Regenerating

The theme files are generated from the Sublime Text 4 Dark VS Code theme in the [Vine](https://github.com/dallasgere/vine) repo:

```bash
python3 scripts/build.py ../vine/themes
```

The script maps each VS Code workbench color to its closest Zed equivalent, resolves every Zed syntax capture against the VS Code `tokenColors` and `semanticTokenColors` rules, and runs a contrast pass so surfaces, dividers, and syntax stay crisp and readable.

## Differences from VS Code

- Zed highlights with tree-sitter rather than TextMate grammars, so some language-specific distinctions collapse to one color per capture.
- Zed theme syntax styles cannot underline or strike through text, so invalid and deprecated code use color only.
