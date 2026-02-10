# .20yk Converter

A lightweight, browser-based utility to package your files into the **.20yk** format.

## Overview

`.20yk` is a strict, lightweight compression format built on top of the standard ZIP structure. It follows the **yk size convention** ($Nyk = 2^N$ bytes), where `.20yk` corresponds to a hard limit of **2²⁰ bytes (1MB)** per internal file.

This tool allows you to:
- Convert standard ZIP files to `.20yk` format.
- Validate that all internal files adhere to the 1MB (2²⁰B) size limit.
- Ensure format compliance automatically.

## Features

- **Client-Side Processing**: No data is uploaded to any server. Everything happens in your browser using [JSZip](https://stuk.github.io/jszip/).
- **Instant Validation**: Quickly checks if your ZIP file meets the `.20yk` specifications.
- **Modern UI**: A sleek, reactive interface with dark mode and glassmorphism.

## Usage

1. Open `index.html` in your web browser.
2. Drag and drop a regular ZIP file into the drop zone.
3. The tool will scan internal files for compliance.
4. If valid, click **Download .20yk** to save your packaged file.

## Specification

The full technical specification for the **yk size naming convention** and the `.20yk` format can be found in [20yk_specification.md](./20yk_specification.md).

