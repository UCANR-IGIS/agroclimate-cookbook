# Notes for Collaborators

## GitHub

commit _cache or not?


## Code Syntax Style Guidelines

Let's try to using the native pipe (|>)

## Quarto Tips

### Callouts

There are five different types of callouts available:
 - note
 - warning
 - important
 - tip
 - caution

For more info see <https://quarto.org/docs/authoring/callouts.html>

### Cross-References

We plan to make the book available as PDF, ePub, and HTML. Therefore, avoid the use of hyperlinks for cross-references to other parts of the book. (Hyperlinks are of course fine for external websites). 

For cross references within the book, use the methods descrbibed [here](https://quarto.org/docs/books/book-crossrefs.html)

## References and Bibliography Tips

### Zotero

To copy-paste a citation from Zotero as BibTeK so you can paste it into `references.bib`:

1. Zotero Windows > Edit > Preferences > Export > Item Format > BibTeX  
2. Select the reference  
3. Edit > Copy as BibTeX  
4. reference.bib > Paste  

### R-packages

To copy the citation for a R package to the clipboard in BibTex format, so you can paste it into `references.bib`, run:

`knitr::write_bib("cimir") |> unlist() |> writeClipboard()`

### In-text citations

Find the key for the citation in references.bib, then add the in-text citation following the examples below. (knitr & pandoc will take care of the rest!)

@ggplot2 really contributed to this effort.
  Becomes: Wickham (2016) really contributed to this effort.

grammar of graphics [@ggplot2].
  becomes: That was an excellent idea (Wickham 2016).

@adams1975[p.33] becomes Adams (1975, p. 33) 

[see @adams1975,p.33] becomes (see Adams, 1975, p. 33)

delineate multiple authors with colon: 
[@adams1975; @aberdeen1958]
becomes
(Aberdeen, 1958; Adams, 1975)

Many variations:

https://inbo.github.io/tutorials/tutorials/r_citations_markdown/#syntax

See also how to document the dependencies

https://docs.google.com/presentation/d/1aookDrahyh683uwC-F8uxmeH-JAG9HVFDUVjec6ilgs/edit#slide=id.g2b72e0d2a93_0_124

