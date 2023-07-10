# language-tasklist

<p align="center">
  <a href="https://github.com/bacadra/atom-language-tasklist/tags">
  <img src="https://img.shields.io/github/v/tag/bacadra/atom-language-tasklist?style=for-the-badge&label=Latest&color=blue" alt="Latest">
  </a>
  <a href="https://github.com/bacadra/atom-language-tasklist/issues">
  <img src="https://img.shields.io/github/issues-raw/bacadra/atom-language-tasklist?style=for-the-badge&color=blue" alt="OpenIssues">
  </a>
  <a href="https://github.com/bacadra/atom-language-tasklist/blob/master/package.json">
  <img src="https://img.shields.io/github/languages/top/bacadra/atom-language-tasklist?style=for-the-badge&color=blue" alt="Language">
  </a>
  <a href="https://github.com/bacadra/atom-language-tasklist/blob/master/LICENSE">
  <img src="https://img.shields.io/github/license/bacadra/atom-language-tasklist?style=for-the-badge&color=blue" alt="Licence">
  </a>
</p>

![language-tasklist](https://github.com/bacadra/atom-language-tasklist/blob/master/assets/language-tasklist.png?raw=true)

Simply tasklist for `TODO`, `*.todo` and `*.tasklist` files. A set of tools has been provided by [tasklist-tools](https://github.com/bacadra/atom-tasklist-tools) package.

A package has been inspired by [tasks](https://github.com/irrationalistic/atom-tasks) package.

## Installation

### Atom Text Editor

The official Atom packages store has been [disabled](https://github.blog/2022-06-08-sunsetting-atom/). To get latest version run the shell command

    apm install bacadra/atom-language-tasklist

and obtain the package directly from Github repository.

### Pulsar Text Editor

The package has compability with [Pulsar](https://pulsar-edit.dev/) and can be install

    ppm install bacadra/atom-language-tasklist

or directly [language-tasklist](https://web.pulsar-edit.dev/packages/language-tasklist) from Pulsar package store.

## Features

* Ticks `☐`, `✔`, `✘` are unicode characters, so it is valid as a plain text document.
* Any line that ends with `:` will be considered a header.
* A indentation doesn't matter and user can use it as like.
* Everything is a text, so comments has no use.
* `pass`, `info`, `math` and `code` markups are supported.

## Customization

A custom CSS can be used to personalize tasklist. An example line-trough `done` and `fail` tasks:

```less
.syntax--tasklist {
  &.syntax--done, &.syntax--fail {
    &.syntax--text {
      text-decoration: line-through;
    }
  }
}
```

# Contributing [🍺](https://www.buymeacoffee.com/asiloisad)

If you have ideas on how to improve the package, see bugs or want to support new features - feel free to share it via GitHub.

See my other packages for Atom & Pulsar Text Editors:
<p align="center">
<a href="https://github.com/bacadra/atom-autocomplete-sofistik"><img src="https://img.shields.io/github/v/tag/bacadra/atom-autocomplete-sofistik?style=for-the-badge&label=autocomplete-sofistik&color=blue" alt="autocomplete-sofistik">
<a href="https://github.com/bacadra/atom-bib-finder"><img src="https://img.shields.io/github/v/tag/bacadra/atom-bib-finder?style=for-the-badge&label=bib-finder&color=blue" alt="bib-finder">
<a href="https://github.com/bacadra/atom-hydrogen-run"><img src="https://img.shields.io/github/v/tag/bacadra/atom-hydrogen-run?style=for-the-badge&label=hydrogen-run&color=blue" alt="hydrogen-run">
<a href="https://github.com/bacadra/atom-image-paste"><img src="https://img.shields.io/github/v/tag/bacadra/atom-image-paste?style=for-the-badge&label=image-paste&color=blue" alt="image-paste">
<a href="https://github.com/bacadra/atom-language-latex"><img src="https://img.shields.io/github/v/tag/bacadra/atom-language-latex?style=for-the-badge&label=language-latex&color=blue" alt="language-latex">
<a href="https://github.com/bacadra/atom-language-sofistik"><img src="https://img.shields.io/github/v/tag/bacadra/atom-language-sofistik?style=for-the-badge&label=language-sofistik&color=blue" alt="language-sofistik">
<a href="https://github.com/bacadra/atom-language-tasklist"><img src="https://img.shields.io/github/v/tag/bacadra/atom-language-tasklist?style=for-the-badge&label=language-tasklist&color=blue" alt="language-tasklist">
<a href="https://github.com/bacadra/atom-linter-ruff"><img src="https://img.shields.io/github/v/tag/bacadra/atom-linter-ruff?style=for-the-badge&label=linter-ruff&color=blue" alt="linter-ruff">
<a href="https://github.com/bacadra/atom-linter-sofistik"><img src="https://img.shields.io/github/v/tag/bacadra/atom-linter-sofistik?style=for-the-badge&label=linter-sofistik&color=blue" alt="linter-sofistik">
<a href="https://github.com/bacadra/atom-navigation-panel"><img src="https://img.shields.io/github/v/tag/bacadra/atom-navigation-panel?style=for-the-badge&label=navigation-panel&color=blue" alt="navigation-panel">
<a href="https://github.com/bacadra/atom-open-external"><img src="https://img.shields.io/github/v/tag/bacadra/atom-open-external?style=for-the-badge&label=open-external&color=blue" alt="open-external">
<a href="https://github.com/bacadra/atom-pdf-viewer"><img src="https://img.shields.io/github/v/tag/bacadra/atom-pdf-viewer?style=for-the-badge&label=pdf-viewer&color=blue" alt="pdf-viewer">
<a href="https://github.com/bacadra/atom-project-files"><img src="https://img.shields.io/github/v/tag/bacadra/atom-project-files?style=for-the-badge&label=project-files&color=blue" alt="project-files">
<a href="https://github.com/bacadra/atom-regex-aligner"><img src="https://img.shields.io/github/v/tag/bacadra/atom-regex-aligner?style=for-the-badge&label=regex-aligner&color=blue" alt="regex-aligner">
<a href="https://github.com/bacadra/atom-sofistik-tools"><img src="https://img.shields.io/github/v/tag/bacadra/atom-sofistik-tools?style=for-the-badge&label=sofistik-tools&color=blue" alt="sofistik-tools">
<a href="https://github.com/bacadra/atom-super-select"><img src="https://img.shields.io/github/v/tag/bacadra/atom-super-select?style=for-the-badge&label=super-select&color=blue" alt="super-select">
<a href="https://github.com/bacadra/atom-tasklist-tools"><img src="https://img.shields.io/github/v/tag/bacadra/atom-tasklist-tools?style=for-the-badge&label=tasklist-tools&color=blue" alt="tasklist-tools">
<a href="https://github.com/bacadra/atom-word-map"><img src="https://img.shields.io/github/v/tag/bacadra/atom-word-map?style=for-the-badge&label=word-map&color=blue" alt="word-map">
</p>
