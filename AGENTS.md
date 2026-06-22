# Project Instructions

## Repository purpose

- This repository is the canonical source for blog audio and video files.
- Production files are served from `https://media.christorng.idv.tw`.
- The sibling `christorng.github.io` repository contains the website and content references.

## URL mapping

- In website content and data files, reference a file with `/blog-media/<path-from-this-repository-root>`.
- Do not write `http://localhost:3001` or `https://media.christorng.idv.tw` directly into website content. Website media components select the origin for the current environment.
- `npm start` serves this repository root at `http://localhost:3001` for local development.

## File changes

- Preserve path casing and URL-encode spaces and non-ASCII filename characters in website references.
- When renaming or moving a media file, update every corresponding `/blog-media/*` reference in the sibling website repository.
- When validating a website reference, URL-decode the part after `/blog-media/` and verify that the resulting path exists in this repository.
