# Simple PDF Viewer Specification

1. Overview

A web-based, client-side PDF viewer designed for reading standard documents and manga/comics. It features drag-and-drop loading, dual-page viewing, and auto-play capabilities with a compact, distraction-free UI.

2. Functional Requirements

2.1 File Loading

Drag & Drop: Users can load a PDF file by dragging and dropping it onto the designated drop zone.

Format Support: Supports standard PDF files.

2.2 View Modes

Single Page Mode: Displays one page at a time.

Spread Mode (Default): Displays two pages side-by-side.

Logic: Handles cover pages (Page 1) individually if needed, then pairs subsequent pages.

Binding Direction:

Left-to-Right (Standard): Pages flow 1 → 2 → 3.

Right-to-Left (Manga): Pages flow 3 ← 2 ← 1 (Used for Japanese comics).

2.3 Navigation

Manual Control: "Prev" and "Next" buttons.

Keyboard Support: Left and Right arrow keys for page navigation.

Page Info: Displays "Current Page / Total Pages".

2.4 Auto-Play

Functionality: Automatically advances to the next page after a set interval.

Configuration: Input field to set the interval in seconds (default: 3s).

Controls: "Start/Stop" toggle button.

Interrupts: Auto-play stops automatically upon:

Reaching the last page.

Manual navigation (button click or key press).

Loading a new file.

2.5 Full Screen

Toggle: Button to enter/exit browser native full-screen mode.

Behavior:

Hides the top control bar completely.

Background color changes to Light Gray (#ccc).

PDF scales to fit the screen dimensions automatically.

3. UI/UX Requirements

3.1 Layout & Design

Compact UI: Control bar height is minimized to maximize reading area.

Language: All UI text is in English.

Visual Style:

Dark grey control bar (#333).

Light grey background for content area (Windowed: #e5e5e5, Full screen: #ccc).

Page Gap: Minimal gap (5px) between pages in Spread mode.

3.2 Responsiveness

Auto-Fit: The PDF scale is dynamically calculated to ensure pages fit entirely within the viewport (width and height) without scrolling if possible.

Resize Handling: The viewer automatically re-renders and re-scales pages when the browser window is resized.

4. Technical Stack

HTML5/CSS3: For structure and styling.

JavaScript: Vanilla JS (ES6+).

Library: PDF.js (v3.11.174) via CDN for PDF rendering.
