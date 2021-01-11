# AutoPDFBookmark
[Markdown PDF](https://github.com/yzane/vscode-markdown-pdf) is great but it doesn't provide bookmarks
so here's a python script to Generate bookmark(outline) according to the CSS file given

## how to use
* specify the CSS for `Markdown PDF' like this:
```
"markdown-pdf.styles": [
    "markdownhere.css"
],
```
`markdownhere.css` is something like

```css
body{
  font-family:"Microsoft Yahei";
  font-size: 14pt;
  line-height: 1.4em;
 }

h1 {
  font-family:"Microsoft Yahei";
  font-size: 28pt;
}

h2 {
  font-family:"Microsoft Yahei";
  font-size: 20pt;
}

h3 {
  font-family:"Microsoft Yahei";
  font-size: 16pt;
}
```

* run `Markdown PDF: Export(pdf)` in vscode, to generate the pdf file `example.pdf`
* run `AutoPDFBookmark.py -f example.pdf -c markdownhere.css` to generate a new pdf file with Bookmarks named 'example_new.pdf'

## Special thanks
* [vscode-markdown-pdf](https://github.com/yzane/vscode-markdown-pdf)
* [PyMuPDF](https://github.com/pymupdf/PyMuPDF)
* [cssutils](https://pypi.org/project/cssutils/)

