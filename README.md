<br/>
<div align="center">
  <img src="https://github.com/thomas861205/vscode-settings/blob/master/cover.png">
</div>
<br/>
<div align="center"> Sick ass IDE makes sick ass codes. </div>

# Table of Contents

- [Basic Things](#basic-things)
  - [Extensions](#extensions)
  - [Open setting](#open-setting)

- [Themes and Icons](#themes-and-icons)
  - [file-icons](#file-icons)
  - [High Contrast](#high-contrast)
  - [One Dark Rain Coat with Sublime Bable](#one-dark-rain-coat-with-sublime-bable)
  
- [Execution](#execution)
  - [Code Runner](#code-runner)
  
- [Python](#python)
  - [Jupyter](#jupyter)
  - [Python extension](#python-extension)
  - [VS Code Jupyter Notebook Previewer](#vs-code-jupyter-notebook-previewer)
  
- [C++](#c++)

#  Basic Things

## Extensions

> One of the features of VScode -- a wide variety of extensions, which makes the programming process efficient and satisfying.

> Easy to browse and install, click the 擴充功能 on the left side.

![](https://github.com/thomas861205/vscode-settings/blob/master/extensions.png)

## Open Setting

> Left click the bottom left GEAR icon, find 設定.

![](https://github.com/thomas861205/vscode-settings/blob/master/setting.png)
 <br/>
 
 > Hover on the left section, and hit 編輯 to customize the settings.
 
![](https://github.com/thomas861205/vscode-settings/blob/master/edit_setting.png)
<br/>

# Themes and Icons

> Left click the bottom left GEAR icon, find 色彩佈景主題/檔案圖示佈景主題 to customize themes/icons.

![](https://github.com/thomas861205/vscode-settings/blob/master/change_theme.png)

> Use arrow keys to preview changed theme.

![](https://github.com/thomas861205/vscode-settings/blob/master/use_arrowkey.png)

## file-icons

> [file-icons](https://marketplace.visualstudio.com/items?itemName=file-icons.file-icons) provides a lot of qute icons.

![](https://github.com/thomas861205/vscode-settings/blob/master/file_icons.png)

## High Contrast

> One of the default theme, which is the theme in all example pictures.

## One Dark Rain Coat with Sublime Bable

> [One Dark Rain Coat]() is a purplish theme, also supports sublime highlights.

![](https://github.com/thomas861205/vscode-settings/blob/master/black_rain.png)

# Execution

## Code Runner

> [Code Runner](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner) enables you to run various of codes,
Python, C/C++ are included. But need to step up compiler or interpreter beforehand.

> press crtl+alt+n or right click and select "run code" to execute. Also support block execution in Python. 

# Python

## Jupyter

> [Jupyter](https://marketplace.visualstudio.com/items?itemName=donjayamanne.jupyter) is a sick extension in vscode.

> It allows you to create cells just like Jupyter Notebook by typing the keywowrd "#%%" in a line.

![]()

## Python extension

> [Python]() is a integrated extension containing linting(語法/排版錯誤提示), Code formatting(自動排版), intellisense(智慧填字), etc.

### Linting recommend: flake8

flake8 is quite strict with the coding style, such as space between operators and operants, docstrings are required in every functions,
unused variables, etc...

![]()

1. type "pip install flake8" in terminal.
2. modify user setting(',' might required).

> enables flake8.

```
"python.linting.flake8Enabled": true
```

> ignores certain warning. Error codes can be found in 問題 (buttom left).

```
"python.linting.flake8Args": [
        "--ignore=E265"
    ]
```

### Code formatting recommend: autopep8

1. type "pip install autopep8" in terminal.
2. modify user setting(',' might required).

> choose formatting package.

```
"python.formatting.autopep8Path": "autopep8",
```

> auto format every you save (crtl+s)

```
"editor.formatOnSave": true
```

## VS Code Jupyter Notebook Previewer

# C++
