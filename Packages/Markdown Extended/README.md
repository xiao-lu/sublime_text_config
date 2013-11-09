# [sublime-markdown-extended](https://github.com/jonschlinkert/sublime-markdown-extended)

> Extends Soda's Monokai and the default markdown styles with additional syntax highlighting for
> [YAML Front Matter](http://assemble.io/docs/YAML-front-matter.html), GitHub Flavored Markdown
> (GFM) and language-specific syntax highlighting inside [GFM "fenced" code blocks](https://help.github.com/articles/github-flavored-markdown#syntax-highlighting)

Although substantial changes have been made, thank you [@aziz](https://github.com/aziz) and other contributors to [Knockdown](https://github.com/aziz/knockdown), for the code for the fenced code blocks.

Get [Monokai Extended](https://github.com/jonschlinkert/sublime-monokai-extended) for better highlighting.

#### [Jump to Examples ↓](#examples)


## Getting Started

### 1. Installation

#### Package Control
If you already have [Package Control](http://wbond.net/sublime_packages/package_control/) installed in Sublime Text:

* Select "Install Package" from the Command Palette: <kbd>Ctrl+Shift+P</kbd> on Windows and Linux or <kbd>⇧⌘P</kbd> on OS X)
* Search for "**Markdown Extended**" and click <kbd>enter</kbd>.


#### Manual Installation
Go to `Preferences -> Browse Packages`, and then either download and unzip this plugin into that directory, or:

``` bash
git clone https://github.com/jonschlinkert/sublime-markdown-extended.git "sublime-markdown-extended"
```

### 2. Activate this Language
**After installing this package**, open a markdown file and switch the language to `Markdown Extended`, using one
of the following methods:

* Select from the list of supported languages in your status bar at the bottom right corner of your editor
* `ctrl + shift + p` and search for "Markdown Extended"

### 3. Make "Markdown Extended" the default
To make `Markdown Extended` the default highlighting for the current extension:

1. Open a file with the extension you want to set a default for (i.e. `.md`)
2. Navigate through the following menus in Sublime Text: `View -> Syntax -> Open all with current extension as... -> Markdown Extended`


<!-- **Handlebars version**

Included in this package is a file named `Markdown Extended.tmLanguage-handlebars`, which provides additional syntax highlighting for Handlebars syntax inside markdown files.

If you use [assemble](http://assemble.io) for generating documentation, sites or components, then activate the Handlebars version instead. To do so, first delete `Markdown Extended.tmLanguage`, then renamed the extension of `Markdown Extended.tmLanguage-handlebars` to just `.tmLanguage`. -->


## Features:
* Support for [YAML Front Matter](http://assemble.io/docs/YAML-front-matter.html)
* Support for [GFM "fenced" code blocks](https://help.github.com/articles/github-flavored-markdown#syntax-highlighting)
* Language-specific syntax highlighting support inside [GFM "fenced" code blocks](https://help.github.com/articles/github-flavored-markdown#syntax-highlighting) for most popular languages (see below for the list of supported languages)
* Syntax highlighting for URLs in text which is auto-linked by GFM
* Proper syntax highlighting for bullets and numbers in ordered/unordered lists
* Proper syntax highlighting for bold and italics by ignoring multiple underscores in words


## Markdown Enhancements
The following examples use the [Monokai Extended](https://github.com/jonschlinkert/sublime-monokai-extended) theme.


## Whitespace

### Significant whitespace
**Whitespace is significant** _only directly before and directly after fenced code blocks_! Following these instructions will ensure that highlighting works properly and consistently.

This is very simple:

* **Add a newline** before and after clode blocks
* **No trailing spaces** after the last code block

If you don't, it won't break your code but it won't always look awesome.

### Comparisons with and without proper whitespace

#### Whitespace before the block
You will need to keep a space above and below fenced code blocks for predictable results with syntax highlighting. For example, this is what it looks like when there is no space before a fenced code block:

![image](https://f.cloud.github.com/assets/383994/782115/470ca012-ea35-11e2-940c-5919386f26bf.png)

This is what it looks like with proper spacing:

![image](https://f.cloud.github.com/assets/383994/782119/5b27105a-ea35-11e2-9ea8-7a195f381d7c.png)

#### Whitespace after the block
Also add a new line after code blocks, but make sure that there is no trailing whitespace next to the bottom fence.

**With a trailing whitespace**

![image](https://f.cloud.github.com/assets/383994/782152/0217cb20-ea36-11e2-8cfd-2ea47136fb0c.png)

**Without a trailing whitespace**

![image](https://f.cloud.github.com/assets/383994/782145/f534f1da-ea35-11e2-8689-d606494f7830.png)




## Examples

## GFM Fenced Code Blocks

### Supported languages

The following languages are highlighted inside fenced code blocks:

_Note that in order for a language to be highlighted properly, you must have the language installed in Sublime Text._

* `c`
* `c++`
* `coffee`
* `css`
* `diff`
* `hbs|handlebars`: requires the Sublime Text [Handlebars](https://github.com/daaain/Handlebars) package
* `html|html5`
* `java`
* `json`
* `js|javascript`
* `less`
* `md|markdown`
* `perl`
* `python`
* `r`
* `ruby`
* `sass`
* `scss`
* `shell|bash`
* `stylus`
* `xml`
* `yaml`


### Turn this:
![image](https://f.cloud.github.com/assets/383994/726869/5f066f14-e13d-11e2-9cdd-118f56a39da5.png)

### Into this:
![image](https://f.cloud.github.com/assets/383994/726871/893061c8-e13d-11e2-9bf5-189d850ccc66.png)


### YAML Front Matter

#### Turn this:
![image](https://f.cloud.github.com/assets/383994/726861/2f03fb2a-e13c-11e2-9df0-cb9514b301fe.png)

#### Into this:
![image](https://f.cloud.github.com/assets/383994/726865/aa2cdb6e-e13c-11e2-89b0-c06923447ec9.png)


### Shell

#### Turn this:
![image](https://f.cloud.github.com/assets/383994/851162/38fc84ae-f496-11e2-9014-81b91da16232.png)

#### Into this
![image](https://f.cloud.github.com/assets/383994/851165/468b3282-f496-11e2-8a2d-ebf6f9c925f6.png)



## Author

**Jon Schlinkert**

+ [http://twitter.com/jonschlinkert](http://twitter.com/jonschlinkert)
+ [http://github.com/jonschlinkert](http://github.com/jonschlinkert)


## Copyright and license
Copyright 2013 Jon Schlinkert

[MIT License](LICENSE-MIT)

