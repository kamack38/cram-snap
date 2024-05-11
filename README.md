# cheatsheet

Simple cheatsheet template for [Typst](https://typst.app/).

## Usage

You can use this template in the Typst web app by clicking "Start from template" on the dashboard and searching for `cheatsheet`.

Alternatively, you can use the CLI to kick this project off using the command

```
typst init @preview/cheatsheet
```

Typst will create a new directory with all the files needed to get you started.

## Configuration

This template exports the `cheatsheet` function with the following named arguments:
- `title`: Title of the document
- `subtitle`: Subtitle of the document
- `icon`: Image that appears next to the title
- `column-number`: Number of columns

If you want to change an existing project ot use this template, you can add a show rule like this at the top of your file:

```typst
#import "@preview/cheatsheet:0.1.0": cheatsheet

#set page(paper: "a4", flipped: true, margin: 1cm)
#set text(font: "Arial", size: 11pt)

#show: cheatsheet.with(
  title: [Cheatsheet],
  icon: image("icon.png"),
)

```
