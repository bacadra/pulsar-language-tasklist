# language-tasklist

![language-tasklist](https://github.com/bacadra/pulsar-language-tasklist/blob/master/assets/example.png?raw=true)

This package provides a simple tasklist for `TODO`, `*.todo`, and `*.tasklist` files.

A set of tools are provided by the [tasklist-tools](https://github.com/bacadra/pulsar-tasklist-tools) package.

## Installation

To install `language-tasklist` search for [language-tasklist](https://web.pulsar-edit.dev/packages/language-tasklist) in the Install pane of the Pulsar settings or run `ppm install language-tasklist`. Alternatively, you can run `ppm install bacadra/pulsar-language-tasklist` to install a package directly from the Github repository.

## Features

- A task is a single line consisting of a tick and text.
- Unicode characters have been used to represent ticks.
- There are several types of ticks:
  | Symbol | Code    | Name   | Description                    |
  |--------|---------|--------|--------------------------------|
  | `▷`    | `U+25B7`| `high` | a high priority pending task   |
  | `☐`    | `U+2610`| `todo` | a normal priority pending task |
  | `✔`    | `U+2714`| `done` | a done/pass/completed task     |
  | `✘`    | `U+2718`| `fail` | a failed/rejected task         |
  | `•`    | `U+2022`| `info` | a notes line                   |
- Any line starting with `#` is a chapter, indentation is not allowed, multilevel is supported.
- Any non-tick line ending with `:` is a header.
- Every line ending with `:` trigger an indentation.
- Support for `~text~`, `*text*`, `_text_`, `$text$` and ``text` `` formats.
- Tasklists can be included using the `tasklist` selector.
- Two space indentation is recommended.
- Outline & folding are provided by [navigation-panel](https://github.com/bacadra/pulsar-navigation-panel).

## Customization

You can customize the tasklist by using custom CSS. Here are some examples:

- Add a line-through to `done` and `fail` tasks:

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

- Change `high` tasks color:

  ```less
  .syntax--tasklist.syntax--high.syntax--text {
    color: red;
  }
  ```

# Contributing

If you have any ideas on how to improve the package, spot any bugs, or would like to support the development of new features, please feel free to share them via GitHub.
