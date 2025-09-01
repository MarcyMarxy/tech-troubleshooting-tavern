# Tech Troubleshooting Tavern

&#x1F916; &#x1F37B; &#x1F469;&#x200D;&#x1F4BB;


## Table of Contents
- [Principles](#principles)
- [WSL VSCode Setup](#wsl-vscode-setup)
- [Git GitHub](#git-github)
- [Debug](#debug)
- [Docstring Formats](#docstring-formats)
- [Markdown](#markdown)
- [LaTeX](#latex)
- [I LIKE](#i-like)
  - [Black](#black)
  - [Sphinx](#sphinx)
- [Useful Links](#useful-links)


## Principles
- MVP (minimum viable product)
- DRY (Don't Repeat Yourself)
- Do One Thing


## WSL VSCode Setup
<!-- TODO -->
For Mac: VSCode+zsh(package install)

## Git GitHub

### wouldn't hurt
```
git --version
git status
```
### routine
```shell
git init
git add .
git commit -m "write some messages"
git push
```


> ```
> Author identity unknown
> *** Please tell me who you are.
> ```


```shell
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
git remote add origin https://github.com/？？？.git
git branch -M main
git push -u origin main
```

*References:*
- [CS50 Seminar: Collaboration and Version Control with Git](https://youtu.be/S-gBbnBDUhA)<br>


### Wrong account
<!-- TODO -->

### Delete all
<!-- TODO -->
```
git remote rm origin
ls 
```


## Debug
Python debugger pdb

```
import pdb
```


Set breakpoint
```
pdb.set_trace()
```


Inspect variables
```
p state
state
n
c
```


Quit
```
q
quit
```


## Docstring Formats
- [Google-style](https://google.github.io/styleguide/pyguide.html#38-comments-and-docstrings)
- [Numpydoc](https://numpydoc.readthedocs.io/en/latest/format.html)


## Markdown
<!-- TODO -->
https://validator.w3.org/#validate_by_input<br>
Emoji Unicode
- [emojipedia](https://emojipedia.org/guide-dog#technical)


## LaTex
TinyTex + LaTex Workshop

> ```
> parskip.sty not found
> ```


```shell
pdflatex --version
tlmgr install parskip
tlmgr install titlesec
```


## I LIKE
### Black
code formatter for Python<br>
### Sphinx
Generate documentation from comments and docstrings using Sphinx. <br>
In terminal, type:


```
sphinx-quickstart
```


Enter basic project information.
In `conf.py`, add:


```
import os
import sys

sys.path.insert(0, os.path.abspath('.'))
sys.path.insert(0, os.path.dirname(os.path.dirname(os.path.abspath(__file__))))

extensions = ['sphinx.ext.autodoc']

autodoc_member_order = 'bysource'

html_theme = 'sphinx_rtd_theme'
```


In `index.rst`, add:
```
.. automodule:: <module name>
   :members:
   :undoc-members:
   :show-inheritance:
   :special-members: __init__
```


In terminal, type:
```
sphinx-apidoc -o docs . -f
```
```
make html
```


In VS Code, use "Live Server" extension to preview.


## Useful Links

### Web safe colors
[https://www.colorhexa.com/web-safe-colors]

### HTTP response status codes
[https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Status]

### True Random Number Generator
[https://www.random.org/]

### Example Domains
- [https://www.iana.org/help/example-domains]
