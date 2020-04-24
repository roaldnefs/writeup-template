# Writeup Template

This repository contains a template for my writeups.

## Installation

Install the required packages:


### Debian

```console
$ sudo apt install texlive texlive-xetex texlive-fonts-recommended \
    texlive-fonts-extra pandoc
```

### Mac OS

```console
$ brew install mactex
```

Install the required **pandoc LaTeX template** called [Eisvogel](https://github.com/Wandmalfarbe/pandoc-latex-template):

1. Download the latest version of Eisvogel template from [the release page](https://github.com/Wandmalfarbe/pandoc-latex-template/releases).

2. Extract the downloaded ZIP archive and open the folder.

3. Move the template `eisvogel.tex` to your pandoc templates folder and rename the file to `eisvogel.latex`. The location of the templates folder depends on your pandoc installation: `$HOME/.local/share/pandoc/templates/` or `$HOME/.pandoc/templates/`.

## Usage

To generate the PDF run the following command or use the supplied `Makefile`:

```console
$ pandoc --from markdown --pdf-engine=xelatex --template eisvogel --listings -o writeup.pdf writeup.md
```
