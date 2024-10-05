# ADMU MS Thesis Template

A repository for using Latex for the Ateneo de Manila University MS Computer Science thesis which follows the rules and guidelines imposed by the university.

## Requirements

* Latex Compiler

## Compiling the Paper

The main entry point of the paper is `main.tex`. You can compile it using the following commands:

```bash
pdflatex --shell-escape main.tex && bibtex main && pdflatex --shell-escape main.tex
```

This will produce a file called `main.pdf`.

For *nix users, you may use the following bash script for convenience:

```bash
./compile.sh
```

## Notes

### On Students with Two Advisers

Use the `discsthesis_updated_double_adv.cls` template. To do this make sure that you change the `\documentclass` line on top of `main.tex` to the appropriate cls file. You can then use the definition `\ThesisCoAdviser{NAME OF COADVISER, Ph.D.}` below `\ThesisAdviser` in the cover page of the manuscript.
