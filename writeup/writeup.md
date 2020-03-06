---
title: "Title"
author: [John Doe]
date: "2020-03-06"
subject: "Subject"
keywords: [tag1, tab2]
subtitle: "Subtitle"
lang: "en"
titlepage: true,
titlepage-text-color: "FFFFFF"
titlepage-color: "0C0D0E"
titlepage-rule-color: "8AC53E"
logo: "placeholder.jpg"
logo-width: 350
toc: true
toc-own-page: true
...

# Writeup Template

This repository contains a template for my writeups.

## Installation

Install the required packages:

```console
$ sudo apt install texlive texlive-xetex texlive-fonts-recommended \
    texlive-fonts-extra pandoc
```

Install the required **pandoc LaTeX template** called [Eisvogel](https://github.com/Wandmalfarbe/pandoc-latex-template):

1. Download the latest version of Eisvogel template from [the release page](https://github.com/Wandmalfarbe/pandoc-latex-template/releases).

2. Extract the downloaded ZIP archive and open the folder.

3. Move the template `eisvogel.tex` to your pandoc templates folder and rename the file to `eisvogel.latex`. The location of the templates folder depends on your pandoc installation: `/Users/USERNAME/.local/share/pandoc/templates/` or `/Users/USERNAME/.pandoc/templates/`.

## Usage

To generate the PDF run the following command or use the supplied `Makefile`:

```console
$ pandoc --from markdown --template eisvogel --listings -o writeup.pdf writeup.md
```

