## Nice HTML Generation for orgmode Documents

I put here a few settings for generating nice HTML documents from
orgmode documents. This repository contains CSS files for
solarized-dark and solarized-light schemes which render HTML documents
with good readability.

The sample org file contains example directives to include for linking
to these CSS files or to embed the styles to generate a self
sufficient HTML file.

To link to the CSS files, use the directive,

```
    #+HTML_HEAD: <link rel="stylesheet" type="text/css" href="css/mystyle.css">
```

To embed the style definitions inside the generated HTML file, use the
following directive instead:

```
    #+INCLUDE: "./style-solarized-dark.org"
    OR
    #+INCLUDE: "./style-solarized-light.org"
```

The contents of the CSS files have been put into solarized-dark.org
and solarized-light.org files so that they can be included inline into
your org file.

To export to a LaTeX file with custom fonts (you need to use XeLaTeX
instead of LaTeX to generate the PDF), use the following directive:

```
    #+INCLUDE: "./style-latex.org"
```

In the sample.org file, you can play with the different options by
enabling the right directive. (Just remove the space character after
the `#` for the directive you want to enable).


