# quarto-experiments-pagedbook

You don't need LaTeX to make a PDF book with Quarto! Use PagedJS imstead.

```bash
# install the pagedjs cli
npm install -g pagedjs-cli

# render the book
quarto render
```

Note that the HTML produced doesn't really break individual chapters up (I've set the `h1`s to have page breaks before them in the CSS). So I've wrapped each chapter body in a div with the `.story` class so that I can easily split it into columns.

You could also set images or plots within the `.story` to `column-span: all` so that they go across the columns for a bit more impact!
