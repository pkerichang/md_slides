# Markdown Slides

This is my setup for generating slides from Markdown, adapted from ELSMD.  See [README_elsmd.md](README_elsmd.md) for original instructions.

## Installation

- Install LaTeX by downloading the installer and install the basic scheme (plain + latex).
  - If you have `sudo` permission and wish to install to `/usr/local`, run the installer with `sudo`.
  - After installation, add `tlmgr` PATH to your own PATH setup as instructed.
  - If you install `tlmgr` with `sudo`, call `tlmgr` with  `sudo env PATH=$PATH tlmgr ...`, so it uses
    your PATH setting to find the executable.

- Install the following packages using `tlmgr`:
  ```
  latexmk biblatex biber beamer pdfjam ragged2e booktabs caption
  textpos pdfpages pdflscape titlesec float biblatex-chicago xstring titling
  ```
- install `pandoc`.
  - For Arch Linux, also install `libxcrypt-compat`, which is required for `biber` to work.

## Tips

- When you want to debug, run `make latex_quiet=""` to enable more verbose latex outputs.