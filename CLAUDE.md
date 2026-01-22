# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static HTML/CSS/JavaScript educational web application - a lesson worksheet viewer for teaching programming concepts. It uses no frameworks, build tools, or package managers.

## Running the Application

The app requires a local HTTP server due to CORS restrictions on fetch:

```bash
python -m http.server 8000
# or
npx http-server
```

Access at `http://localhost:8000`

## Architecture

**Single-page application in `index.html`:**
- Embedded CSS (lines 7-145)
- Embedded JavaScript (lines 194-349)
- `lessonData` object defines available weeks and lessons
- Custom markdown parser splits content by `---` delimiter for step-by-step navigation

**Lesson content structure:**
- Markdown files in `Weeks/Week N/` directories
- Images in `Weeks/Week N/images/`
- Each step separated by `---` in markdown files
- Supported markdown: headers, images, bold (`**text**`), inline code (`` `code` ``)

## Adding New Lessons

1. Add lesson entry to `lessonData` object in `index.html`
2. Create markdown file in appropriate `Weeks/Week N/` directory
3. Add images to `Weeks/Week N/images/`
4. Use `---` to separate steps in the markdown file
