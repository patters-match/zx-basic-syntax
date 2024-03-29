# zx-basic-syntax

ZX BASIC language syntax for editing `.bas` files in [Sublime Text 3](https://www.sublimetext.com) code editor. It also supports regular Sinclair BASIC, and [zmakebas](https://github.com/ohnosec/zmakebas) listings.

![screenshot of ZX BASIC highlighting](images/example.jpg?raw=true)

[ZX BASIC](https://zxbasic.readthedocs.io/en/docs/about/) is an updated BASIC dialect which compiles to optimised Z80 machine code for the ZX Spectrum computer. The [Sublime Text](https://www.sublimetext.com) editor, like the ZX BASIC compiler, runs on Linux, Mac OS, and Windows.

This syntax highlighter does not exhaustively match all BASIC keywords, rather its focus is code clarity. Mariana colour scheme (pictured) is recommended over the default Monokai, since some highlights are invisible in Monokai.


### Highlighting Scope:
- Line numbers, and labels which replace them
- Comment lines, comment blocks
- Strings including all [ZX BASIC escaped characters](https://zxbasic.readthedocs.io/en/docs/syntax/#graphic-characters) and [zmakebas escaped characters](https://github.com/ohnosec/zmakebas#user-defined-graphics-udg)
- To avoid over-colouring, keywords are limited to conditionals and those controlling execution flow
- Sub and Function definitions and calls, although their calls are indistinguishable from array references (and strings without sigils) since the parser does not track objects  
*Hover the mouse pointer over a Sub/Function name to jump to the function definition, and to other mentions*
- Variable types, [numbers](https://zxbasic.readthedocs.io/en/docs/syntax/#numbers), separators, operator symbols, and compiler keywords
- Inline Z80 assembly language, via a dependency on https://github.com/mrcook/Z80Assembly

### Instructions:
- Sublime Text -> Preferences -> Browse Packages... which will show you the User folder location
- Download [`ZX BASIC.sublime-syntax`](https://raw.githubusercontent.com/patters-syno/zx-basic-syntax/main/ZX%20BASIC.sublime-syntax) and [`Z80Assembly.tmLanguage.sublime-syntax`](https://raw.githubusercontent.com/mrcook/Z80Assembly/master/Z80Assembly.tmLanguage.sublime-syntax) to the User folder, ensuring your browser does not add .txt to the filenames
- View -> Syntax -> ZX BASIC!
