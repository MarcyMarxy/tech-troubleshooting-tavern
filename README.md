# Tech Troubleshooting Tavern

&#x1F916; &#x1F37B; &#x1F469;&#x200D;&#x1F4BB;<br>

## Table of Contents
- [WSL+VSCode Setup](#wsl-vscode-setup)
- [Git+GitHub](#git-github)
- [Markdown](#markdown)

## WSL+VSCode Setup
<!-- TODO -->

## Git+GitHub

### wouldn't hurt
```
git --version
git status
```
### routine
```
git init
git add .
git commit -m "write some messages"
git push
```
> ```
> Author identity unknown
> *** Please tell me who you are.
> ```
```
git config --global user.email "you@example.com"
git config --global user.name "Your Name"

git remote add origin https://github.com/？？？.git
git branch -M main
git push -u origin main
```

*References:*
- [CS50 Seminar: Collaboration and Version Control with Git](https://youtu.be/S-gBbnBDUhA)<br>

### 上错号了
<!-- TODO -->

### 整个删除
<!-- TODO -->
```
git remote rm origin
ls 
```
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
```
pdflatex --version
tlmgr install parskip
tlmgr install titlesec
```
## I LIKE
### Black
code formatter for Python<br>
### Sphinx
create manuals<br>
