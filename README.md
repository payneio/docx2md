# docx2md

Convert Word `.docx` files to CommonMark Markdown.

Uses `pandoc` to convert a `.docx` file to standards-compliant CommonMark,
writing `<basename>.md` (and extracting media into `<basename>_media/`). The
Markdown is also echoed to stdout. Requires `pandoc`.

## Usage

```bash
docx2md file.docx                 # Write file.md beside the input
docx2md -o output.md file.docx    # Choose the output file
docx2md --wrap file.docx          # Wrap lines at 100 characters
docx2md --wrap 80 file.docx       # Wrap lines at 80 characters
```

## Install

```bash
uv tool install --editable .
```

## License

Copyright (C) 2026 Paul Payne. Licensed under the GNU AGPLv3 — see [LICENSE](LICENSE).
