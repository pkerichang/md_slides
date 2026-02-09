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
  latexmk biblatex biber beamer pdfjam ragged2e booktabs caption mathspec fontspec
  textpos pdfpages pdflscape titlesec float biblatex-chicago xstring titling xkeyval
  svg transparent catchfile
  ```
- install `pandoc`.
  - For Arch Linux, also install `libxcrypt-compat`, which is required for `biber` to work.

- install `tex-fmt` for formatting .tex files.

## Setup

- Create `template.tex`, which will be the beamer template for your slides.
  - To create a quick example, symlink `template_elsmd.tex` to `template.tex`.  You can also use
    this as the base and make your own modifications.
  - `template.tex` is ignored by git.  This is to prevent committing proprietary slide templates
    to public repo.


## Tips

- Run `make note_slides` to create only slides from notes.

- When you want to debug, run `make note_slides latex_quiet=""` to enable more verbose latex outputs.

- You can use the `-B` flag to force rebuild when running `make`.

- Run `make reallyclean` to clean all files before rebuilding.