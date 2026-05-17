# Eternum-PDF-Generator

Eternum-PDF-Generator is a lightweight web app for generating polished PDF exports of the Eternum story.

## Features

- Loads chapter text and metadata from local files
- Converts content into paginated PDF pages sized at 904×1280
- Supports inline variable parsing such as `namelong` so chapter text renders correctly
- Adds footers with page numbers and chapter metadata
- Lets users preview and download individual chapter PDFs
- Uses `jspdf` for client-side PDF generation without a server

## Usage

1. Open `index.html` in a modern browser.
2. Select a chapter from the UI.
3. Click the download button to save the generated PDF.

## Project structure

- `index.html` — main UI and script for PDF generation
- `jspdf.umd.min.js` — PDF library used in the browser
- `chapters/` — source chapter text files and metadata JSON files
- `eternum.json` — optional project configuration file

## Notes

- The parser now correctly handles the `namelong` variable so the chapter text and metadata display its value instead of skipping the line.
- The tool is designed for offline use and works entirely in the browser.
