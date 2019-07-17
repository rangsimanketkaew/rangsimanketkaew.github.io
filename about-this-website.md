---
layout: page
---

- [About this website](#About-this-website)
  - [Platform and Service](#Platform-and-Service)
  - [Language](#Language)
  - [Other tools](#Other-tools)
  - [Jupyter command-line](#Jupyter-command-line)
    - [Merge multiple .ipynb files into one file](#Merge-multiple-ipynb-files-into-one-file)
    - [Convert .ipynb to .html (by default)](#Convert-ipynb-to-html-by-default)
    - [Convert .ipynb to .html (by default)](#Convert-ipynb-to-html-by-default-1)
    - [Execute notebook and replace file](#Execute-notebook-and-replace-file)
    - [Execute notebook and save as .html file](#Execute-notebook-and-save-as-html-file)
  - [Convert .md to .html](#Convert-md-to-html)
    - [Use markdown2](#Use-markdown2)
  - [Convert .md to .html](#Convert-md-to-html-1)
    - [Use markdown-to-html](#Use-markdown-to-html)
    - [Use pandoc](#Use-pandoc)

## About this website

### Platform and Service

- Github static server
- Jekyll
- Disqus
- MakerWidget
- MailChimp

### Language

- Markdown
- Python
- IPython
- HTML
- CSS

### Other tools

- Jupyter Notebook
- Jupyter Book

### Jupyter command-line

#### Merge multiple .ipynb files into one file

```
pip install nbmerge
```

#### Convert .ipynb to .html (by default)

```
jupyter nbconvert NOTEBOOK.ipynb
```

#### Convert .ipynb to .html (by default)

```
jupyter nbconvert NOTEBOOK.ipynb --to html
```

#### Execute notebook and replace file

```
jupyter nbconvert NOTEBOOK.ipynb --execute
```

#### Execute notebook and save as .html file

```
jupyter nbconvert NOTEBOOK.ipynb --execute --to html

```

### Convert .md to .html

#### Use markdown2

```
pip install markdown2
```

### Convert .md to .html

#### Use markdown-to-html

https://www.npmjs.com/package/markdown-to-html

#### Use pandoc

https://pandoc.org/getting-started.html
