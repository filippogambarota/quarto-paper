# APA 7 Template for Quarto

This template is a simplified and adapted version of the [apaquarto](https://github.com/wjschne/apaquarto) template.

## Installing

```bash
quarto use template filippogambarota/quarto-pdfapa
```

This will install the extension and create an example qmd file that you can use as a starting place for your article.

By default, there is a revision mode where simply wrapping the word, sentence or paragraph using `\brev ... \erev` where `...` is the current text, the text will be colored. The behavior can be changed in the YAML frontmatter with the options `showrevision:` and `revisioncolor:`. Setting to `true` the `showrevision:` argument will highlight all changes in the `revisioncolor:` color. If not specified, the default color is red.
To remove the actual `\brev ... \erev` patterns a simple regex would work. Alternatively the `filor::remove_revision()` function from the `filor` R package can be used.
