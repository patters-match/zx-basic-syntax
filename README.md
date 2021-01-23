# zx-basic-syntax

ZX BASIC language syntax for editing `.bas` files in [Sublime Text](https://www.sublimetext.com) code editor.

![screenshot of ZX BASIC highlighting](images/example.jpg?raw=true)

ZX BASIC is an updated BASIC dialect which compiles to optimised Z80 machine code for the Sinclair ZX Spectrum computer. Sublime Text is a good fit for [Boriel's ZX BASIC compiler](https://zxbasic.readthedocs.io/en/docs/about/) since both software projects will run on Linux, Mac OS, and Windows.

This syntax highlighter has been created using the public ZX BASIC documentation as a guide. It does not exhaustively match all BASIC keywords, rather it focuses on code clarity. Mariana colour scheme (pictured) is recommended over the default Monokai, since some highlights are invisible in Monokai.

- Comments and strings are well implemented. All of the escaped characters described [here](https://zxbasic.readthedocs.io/en/docs/syntax/#graphic-characters) are detected.
- Keyword highlighting is limited to conditionals, and those which impact the flow of the program.
- Sub and Function definitions and calls are highlighted, though the calls are indistinguishable from array references since the parser does not track objects
- Inline ASM code blocks are excluded but the comments within are highlighted.
- Numbers, separators, and non-keyword operators are also in. Compiler keywords too.
- Some additional bits are left commented out, such as all BASIC function keywords, or the ability to use an external ASM syntax file for instance.
