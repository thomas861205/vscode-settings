<br/>
<div align="center">
  <img src="https://github.com/thomas861205/vscode-settings/blob/master/images/cover.png">
</div>
<br/>

<div align="center">:fire: Sick ass IDE makes sick ass codes. ver 1.33.1 :fire:</div>



# Why I switch to VScode?
<!-- Becuse it looks lit af, that's it. -->
Mostly because of Python programming. Sublime has Python REPL, but it is quite slow and apt to crash when executing big programs. In VScode, it has built-in terminal and is stable and fast. Plus, the Jupyter extension is awesome (tho not as good as Jupyter Notebook).
Last but not least, I care about the UI very much. I rock with cool theme and change them frequently, VScode also got it covered.

# Table of Contents

- [Basic Things](#basic-things)
  - [Extensions](#extensions)
  - [Open Setting](#open-setting)
  - [Hot Keybind](#hot-keybind)
  - [Setting Environment Path](#setting-environment-path)

- [Themes and Icons](#themes-and-icons)
  - [file-icons](#file-icons)
  - [Monokai](#Monokai)
  
- [Execution](#execution)
  - [Code Runner](#code-runner)
  
- [Python](#python)
  - [Jupyter](#jupyter)
  - [Python extension](#python-extension)
  - [VS Code Jupyter Notebook Previewer](#vs-code-jupyter-notebook-previewer)
  
- [C++](#c++)

- [Processing](#processing)

#  Basic Things

## Extensions

> One of the features of VScode -- a wide variety of extensions, which makes the programming process efficient and satisfying.<br>
> Easy to browse and install, click the Extensions on the left side.

![](https://github.com/thomas861205/vscode-settings/blob/master/images/extensions.png)

## Open Settings

> Left click the bottom left GEAR icon, find Settings.

![](https://github.com/thomas861205/vscode-settings/blob/master/images/setting.png)
 <br/>
 

## Hot Keybind

- Close Open Folder: press `ctrl+k` then press `f`
- Save File: `ctrl+s`
- Fontsize Up/Down: `ctrl + "numberpad +"` / `ctrl + "numberpad -"`
- Toggle Sidebar: `ctrl+b`
- Open Terminal: `ctrl+`
- Run codes: `F5`

## Setting Environment Path

1. Go to 桌面.

2. Right click 我的電腦, select 內容.

3. Click 進階系統設定 on the left, and select 環境變數 in the new window.

4. Find PATH in 使用者變數(upper section), and edit.

5. Click 確定 all the way out.

# Themes and Icons

> Left click the bottom left GEAR icon, find Color Theme to customize themes/icons.

![](https://github.com/thomas861205/vscode-settings/blob/master/images/change_theme.png)

> Use arrow keys to preview changed theme.

![](https://github.com/thomas861205/vscode-settings/blob/master/images/use_arrowkey.png)

## file-icons

> [file-icons](https://marketplace.visualstudio.com/items?itemName=file-icons.file-icons) is an extension which provides a lot of qute icons.

![](https://github.com/thomas861205/vscode-settings/blob/master/images/file_icons.png)

## Monokai

> One of the default theme, which is the theme in all example pictures. Also, it is the default theme in Sublime Text 3.


# Execution


## Code Runner

> [Code Runner](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner) enables you to run various of codes,
Python, C/C++ are included. But need to set up compiler or interpreter beforehand.<br>
> press `ctrl+alt+n` or right click and select "run code" to execute. Also support block execution in Python. 

![](https://github.com/thomas861205/vscode-settings/blob/master/images/run_code.png)

# Python

## Jupyter

> [Jupyter](https://marketplace.visualstudio.com/items?itemName=donjayamanne.jupyter) is a sick extension in vscode. But in the this version, the feature has been integrated in the [Python](https://marketplace.visualstudio.com/itemdetails?itemName=ms-python.python) extension, so you don't need to download Jupyter.<br>
> It allows you to create cells just like Jupyter Notebook by typing the keyword "#%%" in a line. You can also right click and select "Run Current File in Python Interactive Window".

![](https://github.com/thomas861205/vscode-settings/blob/master/images/jupyter.png)

## <a name="python-extension"></a>Python

> [Python](https://marketplace.visualstudio.com/itemdetails?itemName=ms-python.python) is a integrated extension containing linting(語法/排版錯誤提示), Code formatting(自動排版), intellisense(智慧填字), etc.

### Linting recommend: flake8

flake8 is quite strict with the coding style, such as space between operators and operants, docstrings are required in every functions,
unused variables, etc...

1. type "pip install flake8" in terminal.
2. modify user setting(',' might required).

![](https://github.com/thomas861205/vscode-settings/blob/master/images/flake8.png)

> enables flake8.

```
"python.linting.flake8Enabled": true
```

![](https://github.com/thomas861205/vscode-settings/blob/master/images/error_e226.png)

> ignores certain warning. Error codes can be found in 問題 (buttom left).

```
"python.linting.flake8Args": [
        "--ignore=E226"
    ]
```

### Code formatting recommend: autopep8

1. type "pip install autopep8" in terminal.
2. modify user setting(',' might required).

> choose formatting package.

```
"python.formatting.autopep8Path": "autopep8"
```

> auto format every you save

```
"editor.formatOnSave": true
```

## VS Code Jupyter Notebook Previewer

[VS Code Jupyter Notebook Previewer](https://marketplace.visualstudio.com/items?itemName=jithurjacob.nbpreviewer) let you preview
.ipynb so you don't need to open jupyter notebook. But only preview, cannot execute,

> press "show preview" on the upper right side.

![](https://github.com/thomas861205/vscode-settings/blob/master/images/jupyter_preview.png)

# <a name="c++"></a>C++

> Under construction :hammer:

# Processing

> Processing is a java-based language. Using processing can easily accomplish some visual effects or physical simulation. But it isn't supported by Code Runner by default. We need to set up the processing-java in environment path first.

- [Set up環境變數](#setting-environment-path)

> Find the path of processing-3.3.7 folder, mine is `D:\processing-3.3.7\`. <br>
> Add it to the [PATH](#setting-environment-path).

- Let Code Runner recognize .pde(processing extension).

> Add the code below to the user setting.

```
"code-runner.executorMapByFileExtension": {
    ".pde": "processing-java --sketch=$dir --output=$dir/output --force --run"
},
```
