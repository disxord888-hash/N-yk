# .11yk Converter

A lightweight, browser-based utility to package your files into the **.11yk** format.

## Overview

`.11yk` is a strict, lightweight compression format built on top of the standard ZIP structure. It is designed for packaging small data files while enforcing a hard limit of **1024KB per file**. This ensures that any compliant `.11yk` file remains compact and easy to process.

This tool allows you to:
- Convert standard ZIP files to `.11yk` format.
- Validate that all internal files adhere to the 1024KB size limit.
- Ensure format compliance automatically.

## Features

- **Client-Side Processing**: No data is uploaded to any server. Everything happens in your browser using [JSZip](https://stuk.github.io/jszip/).
- **Instant Validation**: Quickly checks if your ZIP file meets the `.11yk` specifications.
- **Modern UI**: A sleek, reactive interface with dark mode and glassmorphism.

## Usage

1. Open `index.html` in your web browser (or use the GitHub Pages link).
2. Drag and drop a regular ZIP file into the drop zone.
3. The tool will scan internal files for compliance.
4. If valid, click **Download .11yk** to save your packaged file.

## Deployment

### GitHub Pages
This tool is ready to be hosted on GitHub Pages:
1. Upload the contents of this folder to a new GitHub repository.
2. Go to **Settings > Pages**.
3. Under **Build and deployment**, set the source to `Deploy from a branch` and select `main` (or your default branch).
4. Your converter will be live at `https://<your-username>.github.io/<repo-name>/`.

## Specification

The full technical specification for the `.11yk` format can be found in [11yk_specification.md](./11yk_specification.md).

