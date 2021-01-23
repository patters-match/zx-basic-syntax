# zx-basic-syntax

ZX BASIC language syntax for editing `.bas` files in [Sublime Text](https://www.sublimetext.com) code editor.

![screenshot of ZX BASIC highlighting](images/example.jpg?raw=true)

**ZX BASIC** is an updated BASIC dialect which compiles to optimised Z80 machine code for the ZX Spectrum computer. Sublime Text, like [Boriel's ZX BASIC compiler](https://zxbasic.readthedocs.io/en/docs/about/) runs on Linux, Mac OS, and Windows.

This syntax highlighter does not exhaustively match all BASIC keywords, rather it focuses on code clarity. Mariana colour scheme (pictured) is recommended over the default Monokai, since some highlights are invisible in Monokai.

Included:
- Comments and strings, with all escaped characters described [here](https://zxbasic.readthedocs.io/en/docs/syntax/#graphic-characters)
- Keyword highlighting is limited to conditionals, and those which control the flow of the program
- Sub and Function definitions and calls are highlighted, though the calls are indistinguishable from array references since the parser does not track objects
- Inline ASM code blocks are correctly excluded, but the comments within are highlighted
- Numbers, variable types, separators, operator symbols, and compiler keywords are also in
