# zx-basic-syntax

ZX BASIC language syntax for editing `.bas` files in [Sublime Text 3](https://www.sublimetext.com) code editor.

![screenshot of ZX BASIC highlighting](images/example.jpg?raw=true)

**ZX BASIC** is an updated BASIC dialect which compiles to optimised Z80 machine code for the ZX Spectrum computer. [Sublime Text](https://www.sublimetext.com) code editor, like [Boriel's ZX BASIC compiler](https://zxbasic.readthedocs.io/en/docs/about/) runs on Linux, Mac OS, and Windows.

This syntax highlighter does not exhaustively match all BASIC keywords, rather it focuses on code clarity. Mariana colour scheme (pictured) is recommended over the default Monokai, since some highlights are invisible in Monokai.

### Highlight Scope:
- Comment lines, comment blocks, inline assembly comments
- Strings including all [escaped characters](https://zxbasic.readthedocs.io/en/docs/syntax/#graphic-characters)
- To avoid over-colouring, keywords are limited to conditionals and those that control execution flow
- Sub and Function definitions and calls, and although their calls are indistinguishable from array references since the parser does not track objects
- Variable types, [numbers](https://zxbasic.readthedocs.io/en/docs/syntax/#numbers), separators, operator symbols, and compiler keywords

### Instructions:
- Sublime Text -> Preferences -> Browse Packages... which will show you the User folder location
- Download `ZX BASIC.sublime-syntax` from this repository to that folder
- View -> Syntax -> ZX BASIC!
