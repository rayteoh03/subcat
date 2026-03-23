<div align="center">

<img src="https://em-content.zobj.net/source/apple/391/cat-face_1f431.png" width="80" alt="SubCat">

# SubCat

**Subtitle line formatter for Mandarin & Cantonese scripts**

Paste a paragraph. Get subtitle lines. Export .SRT.

No install · No server · Fully offline

[**→ Open SubCat**](https://YOUR_USERNAME.github.io/YOUR_REPO_NAME)

</div>

---

## What it does

SubCat takes paragraph-form Chinese scripts and splits them into properly sized subtitle lines — ready to export as `.SRT` files for your NLE.

It's a single HTML file that runs entirely in your browser. Nothing is uploaded, nothing leaves your device.

## Features

**Smart line splitting** — Splits at natural punctuation breaks first, then by character width. Uses your browser's built-in Chinese word segmentation (`Intl.Segmenter`) so it never breaks in the middle of compound words like 圖書館 or 幼稚園.

**Dialogue quote removal** — Automatically detects and strips attributed dialogue (`說：「...」`, `表示：「...」`) from news and documentary scripts. Keeps standalone `「...」` intact.

**ENPS stripping** — Removes newsroom markup: `{...}`, `<...>`, `[...]`, `((...))`, and `*...*` markers.

**Punctuation modes** — Strip all, keep all, or strip CJK only. Numbers like `1.8` and `2,000` are always preserved.

**Line merging** — Click to merge short adjacent lines. Merges apply as global rules across repeated pairs.

**Preview & navigation** — Click any preview line to jump to the source text. Color-coded badges show which lines are within limits.

**Export** — `.SRT` with timecodes, `.TXT` plain text, or copy to clipboard.

**Undo / Redo** — Up to 50 states. `Ctrl+Z` / `Ctrl+Shift+Z`.

**Built-in manual** — Click 📖 Manual for a cat-narrated walkthrough of every feature.

## Browser support

Works in any modern browser with `Intl.Segmenter` support:

| Browser | Version |
|---------|---------|
| Chrome | 87+ |
| Safari | 15.4+ |
| Firefox | 125+ |
| Edge | 87+ |

Older browsers still work — word-aware splitting gracefully reverts to character-level splitting.

## Usage

1. Open `index.html` in your browser (or visit the GitHub Pages link)
2. Paste your script in the left panel
3. Adjust settings if needed (max chars, punctuation mode, etc.)
4. Export as `.SRT`, `.TXT`, or copy lines

## Deploy

SubCat is a single `index.html` file. To host it:

1. Fork or clone this repo
2. Enable GitHub Pages (Settings → Pages → Deploy from branch → `main`)
3. Done — your site is live at `https://your-username.github.io/repo-name`

## License

MIT

---

<div align="center">
<sub>There's a fish somewhere. The cat is hungry. 🐟</sub>
</div>
