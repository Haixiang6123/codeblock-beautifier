# Code Block Beautifier

<p align="center">
    <img width="200" src="screenshot/icon-origin.png">
</p>

A chrome extension for beautifying code blocks in any websites that have `<pre><code>...</code></pre>` structure.
Thanks to [highlight.js](https://highlightjs.org/), I don't need to write so many codes for language detection and tons of themes 😂.

You can watch a [video]() to preview it.

## Screenshot

![Scrrenshot](screenshot/effect.png)

## Install & Download

Check [this](https://chrome.google.com/webstore/detail/code-block-beautifier/gpcjjddhdnilcbddlonlfgdbejfboonn) on Chrome app store.

or

[Download from ./dist/codeblock-beautifier.crx](./dist/codeblock-beautifier.crx) it anyway.

## How to use

![How to use](screenshot/how-to-use.png)

## Features

* ⚒ Beautify any code blocks wrapping in `<pre/>` automatically. 

* 🧲 Beautify code blocks according to your languages preference.

* 🔓 Auto detect what languages that the author defines

* 🎁 Supporting [Medium](https://medium.com/), [StackOverflow](https://stackoverflow.com/),
[简书](https://www.jianshu.com/), [知乎](https://www.zhihu.com/), [W3C Plus](https://www.w3cplus.com/).

* 🎉 More than 80 themes are available. Can switch to any language highlight solutions.

* 🎊 More than 20 language highlight themes are available. Can switch to any highlight themes you like.

## Purpose
The main reason I develop it it because [Medium](www.medium.com) doesn't provide a good highlight code blocks.
Well, I know there are several ways to embed codes in it, but some people (like me) don't wanna create a gist or code sandbox project to put codes on my block. So most of time, I see this 🙄:

![No highlight](screenshot/notHighlight.png)

What I expect should be like this 😄:

![Highlight](screenshot/highlight.png)

So I build an extension to beautify code blocks in [Medium](www.medium.com).

It does beautify all code blocks. It can also be used for other websites that contain `<pre/>`.
The only thing you need to do is to press the "Parse" button!

## Future
There may have some problems that I haven't found for this extension yet. If you have any questions or find any bugs, please put an issue on this repo. Thank you!

## Change Log

### v1.0

* Add parsing action. It is able to parse code blocks and apply given theme.

* Add styles to beautify each code blocks.

### v1.0.1

* Enable user to select highlight languages with adding a panel below code blocks. 

* Enable user to select different theme and apply to all code blocks.

### v1.0.2

* Enable user to select highlight languages preference. Because highlight.js may detect wrong languages,
setting highlight languages preference can let it detect correctly.

* Add revert action. User can revert parsed code blocks to original styles.

### v1.0.3

* Add background color of theme to inline style of `<code/>` to adapt most websites.

* Add auto detection for those websites that have already defined what languages should be highlighted.

* Add auto parsing action.

* Fix bugs:

    * Remove loading CSS files at the beginning
    
    * Compatible with some websites that have CSS styles on `<pre/>` or `<code/>`
    
    * Reverting to original HTML elements.
    
    * Can switch language preference immediately.
    
### v1.0.4

* Update to a new UI. Switching to "Codes" styles from plain HTML element.

* Fix bugs:
    
    * Enable to cover original styles with hljs for Popup page.
    
    * Add event hub to notify all components in Popup page.
    
    * Enable to detect language by checking attributes of `<pre/>` and `<code/>`.
