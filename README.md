# Thesis book project

A Quarto book project rendering to Typst (PDF). See `_quarto.yml` for
the chapter list and format options.

## Rendering

Open `thesis-book.Rproj` in RStudio, then use the Build pane's Render
Book button, or from a terminal in this folder:

    quarto render

If RStudio's Build pane doesn't show a Render Book option, go to
Tools > Project Options > Build Tools and set the project type to
Quarto.

Native Typst support for Quarto *book* projects is recent (Quarto
1.9+). Check your version with `quarto --version` and update from
https://quarto.org/docs/get-started/ if needed. By default, a book
rendered with `format: typst` uses Quarto's bundled "orange-book"
extension, which has a decorative textbook look (coloured chapter
headers, sidebars). That may not match the formatting your university
requires for thesis submission, so check that early and look at
Quarto's Custom Typst Formats docs, or an existing dissertation-style
extension, if you need to change it.

## Private notes

The `notes/` folder is listed in `.gitignore` and is never committed
or pushed. See `notes/README.md`.

## Structure

    index.qmd               Preface / abstract
    01-introduction.qmd
    02-literature-review.qmd
    03-methodology.qmd
    04-analysis.qmd
    05-discussion.qmd
    06-conclusion.qmd
    references.qmd
    references.bib
    notes/                  Private, gitignored
