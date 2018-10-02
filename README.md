# Vython
Use Vim as a Python shell--like Jupyter but it's in Vim.

Features:

-Executes Python files, individual lines, or blocks (via visual mode) within the Vim editor  
-Displays the output in a separate buffer/window  
-Can inspect variable/expression values  
-Set breakpoints within functions etc. and inspect local variables  
-Completions (via IPython if available, else rlcompleter)  



Requirements:

-Vim (gVim, neovim, Oni) with Python3 build (Python2 not supported, nor will it be); ' :echo has("python3") ' must return 1


-----------------
Default bindings/commands:
-----------------
:Vython   ---initialize Vython, create new pane/buffer for outputs  
\<F10\>     ---same as above  
  
\<F5\>      ---execute entire file  
\<s-enter\> ---execute current line or selected region (if in visual mode)  
\<c-b\>     ---try to evaluate expression in line, or stuff before = (i.e., if the line has x = 2, will output the CURRENT value of x, which may or may not be defined)  
  
\<c-u\>     ---get completions (if in insert mode)  

Demo/tutorial is in the works.
