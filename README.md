<div align="center">

# ✦ Poetry Writer

### A free, browser-based poetry tool with live rhyme suggestions

**[▶ Open the App](https://yourusername.github.io/poetry-writer)**

![HTML](https://img.shields.io/badge/HTML-Pure-c49a55?style=flat-square&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla-1a1208?style=flat-square&logo=javascript)
![No Dependencies](https://img.shields.io/badge/Dependencies-None-4a6741?style=flat-square)
![Free](https://img.shields.io/badge/Hosting-Free%20Forever-8b3a1a?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-c084fc?style=flat-square)

</div>

---

## What is it?

Poetry Writer is a distraction-free writing tool that helps you compose poems with real-time rhyme suggestions. As you write each line, you can tag any word with `#` to instantly see words that rhyme with it — complete with definitions — so you always have inspiration ready for your next line.

There is nothing to install, no account to create, and no cost. It runs entirely in the browser as a single HTML file, calling the free [Datamuse API](https://www.datamuse.com/api/) for rhyme lookups.

---

## Features

| Feature | Description |
|---|---|
| **Split-screen layout** | Write on the left, see your growing poem on the right — always in view |
| **Inline rhyme lookup** | Put `#` after any word to see rhymes and their definitions |
| **Multiple triggers** | Use several `#` symbols in one line to look up multiple words at once |
| **Live poem view** | Your poem updates line by line as you write, typeset in an editorial serif font |
| **Save to file** | Download your finished poem as a `.txt` file with one click |
| **Undo** | Remove the last line at any time |
| **Zero cost** | No API key, no server, no subscription — runs entirely in the browser |

---

## How to Use

**1. Write a line**
Type your line into the input field at the top left.

**2. Tag words for rhymes**
Put `#` directly after any word you want rhymes for:

```
The cat# sat beside the fire,
```

You can tag multiple words in one line:

```
The night# was dark and full of light#,
```

**3. Press Enter**
Your line is added to the poem on the right. Rhyme suggestions appear below the input, each with its definition — useful context for choosing the right word.

**4. Write the next line**
Use the rhyme suggestions as inspiration when writing your rhyming couplet or next stanza. The `#` symbols are stripped from your poem automatically — they never appear in the final text.

**5. Save**
Click **Save Poem** in the header to download your poem as a `.txt` file.

---

## Example

You type:

```
The old man walked beneath the moon#,
```

The rhyme panel shows:

| Word | Definition |
|------|------------|
| tune | A melody or musical phrase |
| spoon | A utensil with a shallow bowl |
| June | The sixth month of the year |
| soon | In a short time from now |
| boon | A thing that is helpful or beneficial |

You then write the next line knowing exactly what rhymes with *moon*.

---

## Technical Overview

Built as a single self-contained `index.html` file with no external dependencies beyond Google Fonts.

```
index.html
├── HTML  — split-pane layout with left (editor) and right (poem view) panels
├── CSS   — editorial design using Playfair Display, EB Garamond, Cormorant Garamond
└── JS    — rhyme fetching, poem state management, save-to-file
```

**Rhyme data** comes from the [Datamuse API](https://www.datamuse.com/api/) — a free, open, no-key-required lexical API. The browser calls it directly; there is no backend.

**Hosting** is via [GitHub Pages](https://pages.github.com/) — a free static hosting service. The file is served directly from this repository with no build step.

---

## Running Locally

No build tools or installs needed. Just open the file:

```bash
# Clone the repo
git clone https://github.com/yourusername/poetry-writer.git

# Open in browser (Mac)
open index.html

# Open in browser (Windows)
start index.html

# Open in browser (Linux)
xdg-open index.html
```

Or simply drag `index.html` into any browser window.

---

## Project Background

This project started as a Python terminal application, went through a PyQt5 desktop GUI phase, and was ultimately rebuilt as a web app for maximum accessibility. The goal throughout was to keep the tool completely free to use and easy to share — no barriers between a writer and their words.

The design takes an editorial, literary aesthetic — cream paper tones, ink-dark accents, and serif typography — to feel like a real writer's desk rather than a generic productivity tool.

---

## License

MIT — free to use, fork, and modify.

---

<div align="center">

Made with care &nbsp;✦&nbsp; [Open the App](https://yourusername.github.io/poetry-writer)

</div>
