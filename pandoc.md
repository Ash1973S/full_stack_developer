# PANDOC Markdown to PDF

When using `pandoc` with `typest` to convert markdown document to PDF, the fallback
font need to be explicitly defined.

```bash
pandoc README.md -o resume.pdf --pdf-engine=typst -V mainfont="Libertinus Serif"
```

Or if frequently used, create an alias, in `bashrc` or `zshrc`.

```bash
alias md2pdf='pandoc -o resume.pdf --pdf-engine=typst -V mainfont="Libertinus Serif"'
```
