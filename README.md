# vim-aftercolors
Provides support for after/colors/ scripts

This is a mirror of the unmaintained scripts by Peter Hodge at
http://www.vim.org/scripts/script.php?script_id=1641,
to provide support for importing using vim-plug and other plugin managers.

It is currently up to date with the posted v1.3 (2008)

## Description (By Peter Hodge)
Allows you to create an after/colors/ script for customizing any colorscheme. 

-- EXAMPLE -- 
If you like the 'desert' colorscheme, but you really want comments to be red and functions to be blue, previously you would copy the entire colorscheme into your home directory and customize it.  With this plugin installed, you can create a small script to change just the parts you want for that colorscheme, exactly how you would for an ftplugin or syntax script: 

For unix systems you would create: 
  ~/.vim/after/colors/desert.vim: 
    highlight Comment guifg=Red ctermfg=Red 
    highlight Function guifg=Blue ctermfg=Blue 

On windows you would create: 
C:\Documents and Settings\Peter\vimfiles\after\colors\desert.vim: 
    highlight Comment guifg=Red ctermfg=Red 
    highlight Function guifg=Blue ctermfg=Blue 


-- VERSION 6 WARNING -- 
If your Vim is older than version 7, then the after/colors scripts will only be loaded once when Vim starts.  This will not be a problem if you choose your colorscheme in your .vimrc file, but if you change your colorscheme after vim has loaded then your after/colors scripts will be ignored.  This is not an issue in Vim 7. 


In case of problems, you can email me: <toomuchphp-vim at yahoo.com> 
 
install details
1) Put AfterColors.vim in ~/.vim/plugin/ or $HOME\vimfiles\plugin\ 
2) Create your colorscheme customizations in after/colors/<colors_name>.vim 
3) Create global customizations (for all colorschemes) in after/colors/common.vim
