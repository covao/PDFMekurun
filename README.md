# Overviews

A lightweight, client-side web application designed for reading PDF documents and manga directly in the browser. It offers a distraction-free environment with intuitive controls and responsive design.
[Start PDF Viewer](https://covao.github.io/PDFMekurun/PDFMekurun.html)

# Features

🖱️ Drag & Drop: Instantly load local PDF files.

📖 Spread View: Display two pages side-by-side (default).

🔄 Binding Direction: Toggle between Left-to-Right (Standard) and Right-to-Left (Manga) modes.

▶️ Auto-Play: Hands-free page turning with customizable intervals.

🖥️ Full Screen: Immersive reading mode with auto-scaling.

🔗 URL Support: Open specific PDFs and pages via URL parameters.

# Usages

Open the App: Open index.html in any modern web browser.

Load a File: Drag and drop a PDF file into the drop zone.

Navigate:

Click: Use "Prev" / "Next" buttons.

Keyboard: Use ← / → arrow keys.

URL Parameters:

Syntax: ?pdf=[URL]&page=[Number]

Example: index.html?pdf=https://example.com/comic.pdf&page=3

Note: The server hosting the PDF must support CORS.

# Specification

Architecture: Single-page application (SPA).

Tech Stack: HTML5, CSS3, Vanilla JavaScript (ES6+).

Library: PDF.js (v3.11.174).

Compatibility: Works in Chrome, Edge, Firefox, and Safari.

