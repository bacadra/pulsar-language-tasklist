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

![language-tasklist](https://github.com/bacadra/atom-language-tasklist/blob/master/assets/example.png?raw=true)

This package provides a simple tasklist for `TODO`, `*.todo`, and `*.tasklist` files.

A set of tools are provided by the [tasklist-tools](https://github.com/bacadra/atom-tasklist-tools) package.

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

- A task is a single line that consists of a tick and text.
- Unicode characters has been used to represent ticks.
- A few types of ticks are available:
  - `▷` | `U+25B7`| `high`: a high priority pending task,
  - `☐` | `U+2610`| `todo`: a normal priority pending task,
  - `✔` | `U+2714`| `done`: a done/pass/completed task,
  - `✘` | `U+2718`| `fail`: a failed/rejected task.
  - `•` | `U+2022`| `info`: a notes line,
- Any line starting with `#` is a chapter, indentation is not allowed, multilevel are supported.
- Any line ending with `:` is a header.
- Supports of `~text~`, `*text*`, `_text_`, `$text$`, and `` `text` `` formats.
- Tasklists can be injected using the `tasklist` selector.
- Two spaces indentation of tasks recommended.
- An outline & folding are provided by [navigation-panel](https://github.com/bacadra/atom-navigation-panel).

## Customization

You can customize the tasklist by using custom CSS. Here are some examples:

- To add a line-through effect to `done` and `fail` tasks text:

  ```less
  .syntax--tasklist {
    &.syntax--done, &.syntax--fail {
      &.syntax--text {
        text-decoration: line-through;
      }
    }
  }
  ```

- Set bold font-weight of chapters:

  ```less
  .syntax--tasklist {
    &.syntax--chapter {
      font-weight: bold;
    }
  }
  ```

- Change color of high tasks to eye-catching:

  ```less
  .syntax--tasklist.syntax--high.syntax--text {
    color: red;
  }
  ```

# Contributing [🍺](https://www.buymeacoffee.com/asiloisad)

If you have any ideas on how to improve the package, spot any bugs, or would like to support the development of new features, please feel free to share them via GitHub.
