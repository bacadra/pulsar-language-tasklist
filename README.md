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

The official Atom packages store has been [disabled](https://github.blog/2022-06-08-sunsetting-atom/). To obtain the latest version, please run the following shell command:

```shell
apm install bacadra/atom-language-tasklist
```

This will allow you to directly download the package from the GitHub repository.

### Pulsar Text Editor

The package is compatible with [Pulsar](https://pulsar-edit.dev/) and can be installed using the following command:

```shell
ppm install bacadra/atom-language-tasklist
```

Alternatively, you can directly install [language-tasklist](https://web.pulsar-edit.dev/packages/language-tasklist) from the Pulsar package store.

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

If you have any ideas on how to improve the package, spot any bugs, or would like to support the development of new features, please feel free to share them via GitHub.
