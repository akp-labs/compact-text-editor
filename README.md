# Compact Text Editor

A lightweight, browser-based text editor built using pure HTML, CSS, and JavaScript.
It is designed for quick note-taking, rich-text formatting, and instant export as a standalone HTML file.

Compact Text Editor provides a minimal, dependency-free writing environment with live editing, formatting controls, and offline usability. It follows a modular development structure with a single-file distributable build for portability.

---

⚠️ Disclaimer
This project is intended for educational and experimental purposes only. It is not a full-scale word processor or collaborative editor. Some features may be limited, and behavior may vary across browsers.

---

## Usage

### Option 1 — Quick Use (Recommended)

1. Download `dist/compact-text-editor.html`
2. Open it in any browser
3. Start editing immediately

* Works offline.
* No installation required.

---

### Option 2 — Development Mode

1. Clone the repository
2. Open:

```
src/index.html
```

3. Edit files inside the `src/` directory
4. Build the project when needed:

```
python scripts/build.py
```

Recommended for development, customization, and learning.

---

## Features

* Rich text editing using a `contenteditable` container
* Inline formatting using native DOM Range and Selection APIs
* Text styling:

  * Bold, Italic, Underline
  * Strikethrough and highlight
  * Superscript and subscript
  * Inline code formatting
* Font controls:

  * Font family selection
  * Font size adjustment
  * Text color picker
* Text alignment options (left, center, right, justify)
* Live word and character counter
* Partial and full-text formatting support
* Clear formatting without deleting content
* Reset editor with confirmation
* Export content as a standalone HTML file
* Fully offline and self-contained

---

## Project Structure

```
compact-text-editor/
│
├── index.html              # Entry / landing page (GitHub Pages)
│
├── src/                    # Development source code
│   ├── index.html
│   ├── script.js
│   └── style.css
│
├── dist/                   # Final build (for users)
│   └── compact-text-editor.html  # Single-file app
│
├── scripts/                # Build tools
│   └── build.py
│
├── README.md
├── LICENSE
└── .gitignore
```

---

### Build System

Run:

```
python scripts/build.py
```

This will:

* Combine HTML, CSS, and JavaScript
* Bundle everything into a single file
* Output the final build into the `dist/` directory

---

## Architecture Overview

This project uses two modes:

### Development Mode

* Modular structure inside `src/`
* Easy to edit and extend
* Suitable for learning and experimentation

### Production Mode

* Single-file build inside `dist/`
* Fully portable
* Works offline without dependencies

---

## Technology Stack

* HTML5
* CSS3
* Vanilla JavaScript (DOM & Selection APIs)
* Python (build tooling only)

---

## Limitations

* Not intended for collaborative editing
* No advanced document model (HTML-based formatting only)
* No built-in undo/redo beyond browser defaults
* Browser-dependent behavior may vary

---

## Live Demo

Try it here:
https://akpandey-dev.github.io/compact-text-editor

---

## Contributing

* Open for learning and experimentation
* Bugs may exist
* Improvements and suggestions are welcome

---

## License

This project is open for learning, modification, and experimentation.
