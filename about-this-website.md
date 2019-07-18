---
layout: page
---

## About this website

---

- [About this website](#about-this-website)
  - [Platform and Service](#platform-and-service)
  - [Programming language](#programming-language)
  - [IDE and extensions](#ide-and-extensions)
  - [Other tools](#other-tools)
  - [Jupyter command-line](#jupyter-command-line)
  - [Convert .md to .html](#convert-md-to-html)

### Platform and Service

- Github
- Jekyll
- Disqus
- MailChimp
- MakerWidget

### Programming language

- Markdown
- Ruby/Gem
- HTML/CSS
- Python
- IPython notebook

### IDE and extensions

- Visual Studio Code
  - Markdown All in one
  - Markdown Shortcuts
  - markdownlint
  - Live Server
  - Live Server Preview
  - File Utils
  - Auto Close Tag
  - Auto Rename Tag
  - Bracket Pair Colorizer
- Vi/Vim
  - NERDTree

### Other tools

- Jupyter Notebook
- Jupyter Book
- [nbviewer](https://nbviewer.jupyter.org/)

### Jupyter command-line

- Merge multiple .ipynb files into one file

```
pip install nbmerge
```

- Convert .ipynb to .html (by default)

```
jupyter nbconvert NOTEBOOK.ipynb
```

- Convert .ipynb to .html (by default)

```
jupyter nbconvert NOTEBOOK.ipynb --to html
```

- Execute notebook and replace file

```
jupyter nbconvert NOTEBOOK.ipynb --execute
```

- Execute notebook and save as .html file

```
jupyter nbconvert NOTEBOOK.ipynb --execute --to html
```

### Convert .md to .html

- Use markdown2

```
pip install markdown2
```

- Use markdown-to-html

https://www.npmjs.com/package/markdown-to-html

- Use pandoc

https://pandoc.org/getting-started.html
