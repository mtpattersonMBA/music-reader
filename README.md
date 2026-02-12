# PDF Focus Reader

A lightweight web app that uses **PDF.js** to load a local PDF and render every page in one vertically scrollable view. It also includes a **Focus Mode** overlay with a movable focus band that magnifies only the band area.

## Features

- Load a local PDF file from your machine.
- Render all pages in a single vertical scroll.
- Toggle Focus Mode on/off.
- Move the focus band up/down.
- Set focus zoom to `1.0x`, `1.5x`, or `2.0x`.

## Exact run steps

1. Open a terminal in this project directory.
2. Start a local static server:

   ```bash
   python3 -m http.server 8000
   ```

3. Open your browser to:

   ```
   http://localhost:8000
   ```

4. Click **Load PDF** and choose a local `.pdf` file.

## Controls

- **Load PDF**: Select and render a local PDF.
- **Toggle Focus Mode**: Show/hide the magnified focus overlay.
- **Focus Band Up**: Move focus band upward.
- **Focus Band Down**: Move focus band downward.
- **Zoom 1.0x / 1.5x / 2.0x**: Set magnification level for focus band.

## Simple smoke test

1. Run the app using the steps above.
2. Load any multi-page PDF.
3. Confirm all pages appear in one vertical column.
4. Click **Toggle Focus Mode** and verify a centered highlighted band appears.
5. Click **Focus Band Up** / **Focus Band Down** and confirm the band moves.
6. Switch zoom levels between `1.0x`, `1.5x`, and `2.0x` and verify the band magnification changes.
7. Scroll the document and verify the focus band continues magnifying the on-screen content beneath it.
