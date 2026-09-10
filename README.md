# Typewriter no.01

A clear-shell typewriter on a studio table that answers questions about Yanice Yang's work. It is the About page of her portfolio, built as a conversation: the sheet of kraft paper is the interface, the keys and knobs are the controls.

- One file, no framework: `index.html` holds the styles, the markup, the script and the print-only résumé.
- The machine is a real CSS 3D scene (frosted acrylic body, glass inspection window, chrome fittings, matte plastic keys) following the Glass Objects design system, see `DESIGN.md`.
- Key sounds are synthesized in the browser with the Web Audio API. Nothing is downloaded except two Google Fonts (Jost, Special Elite).
- Type on your keyboard, or click the keys. Return submits. Three preset questions are typed onto the sheet at the start; anything else is matched by keyword.

## Run

Open `index.html` in a browser, or serve the folder with any static server. To embed in a portfolio, use it as a route or an `<iframe>` and point the `← back` link at the home page.

## Customise

All in `index.html`:

- `IMAGES` at the top of the script: URLs of screenshots to show on the sheet.
- `C`: every line the machine types.
- `ROWS`: the key layout.
- `route()`: which keywords lead to which answer.
- `#print-resume`: the two-page résumé that prints when the visitor asks for it.

## License

The code in this repository is released under the [MIT License](LICENSE).

The résumé text, the name, and any images or personal material shown on the sheet or in the print-only résumé are Yanice Yang's own content and are not covered by that license. If you reuse the typewriter, replace `C`, `#print-resume` and `IMAGES` with your own content.
