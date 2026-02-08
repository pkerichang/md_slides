# Markdown Slides

This is my setup for generating slides from Markdown, adapted from ELSMD.  See [README_elsmd.md](README_elsmd.md) for original instructions.

## Installation

- Install LaTeX by downloading the installer and install the basic scheme (plain + latex).
- Install the following packages using `tlmgr`:
  ```
  latexmk biblatex beamer pdfjam ragged2e booktabs caption
  textpos pdfpages pdflscape titlesec float biblatex-chicago xstring titling
  ```
- install `pandoc`.

## Tips

- When you want to debug, run `make latex_quiet=""` to enable more verbose latex outputs.