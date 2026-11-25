> **Note:** This project, including the code and this README, was generated with AI assistance (Anthropic's Claude) and reviewed by a human. Check the output before relying on it.

# ST Beautifier

A single-file, offline tool that highlights and formats **IEC 61131-3 Structured Text**. It handles Rockwell Studio 5000 ST, Beckhoff TwinCAT ST and Siemens SCL.

Open `index.html` in a browser, paste your code, and press **Format**. There's nothing to install, no build step and no network access.

## Features

- **Syntax highlighting** in both the input and output panes, in light and dark themes.
- **Formatting** that changes only whitespace, line breaks and keyword casing. It never adds, removes or reorders tokens, so the code behaves exactly as before.
- **Settings for:**
  - line breaking (long conditions, calls with many parameters, one statement per line)
  - indentation (tabs or spaces, `CASE` labels, `VAR` blocks)
  - alignment of `:`, `:=`, `=>` and trailing comments
  - spacing and keyword casing
  - blank lines, including around regions and `(* ... *)` comment sections
- **Live preview** in the settings dialog. Changing a setting reformats the input immediately, and Ctrl+Z undoes it.
- **Code reading aids:** folding for `IF`, `CASE`, loops, `VAR` and regions. Hovering a block keyword highlights its partner, and clicking a name highlights every occurrence.
- **Export / Import** of settings as JSON, so a team can share one style.

## Privacy

Your code never leaves the browser. Nothing is uploaded, and pasted code is never stored. Only the formatting settings are saved, in your browser's `localStorage`.

## Use

- **Online:** open the GitHub Pages link for this repository.
- **Offline:** download `index.html` and double-click it.

## Limitations

- It's a reading and formatting aid, not a compiler. It does no syntax checking, and anything it doesn't recognise is passed through unchanged.
- It's tested mainly in current Edge, Firefox and Chrome.

## License

MIT. See the notice at the top of `index.html`.
