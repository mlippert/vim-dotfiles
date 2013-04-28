vim-dotfiles
============

My configuration files for vim

Create links .vimrc -> .vim/rc/vimrc and .gvimrc -> .vim/rc/gvimrc

Make sure that the directory .vim/tmp exists for storing backup files

uses pathogen to install plugins located in .vim/bundle
Those plugins are submodules
- supertab
- vim-colors-solarized
- vim-jsbeautify

I have edited the .vim/javascript.vim file I originally got from
http://vadconf.googlecode.com/svn/trunk/vim/syntax/javascript.vim

I see others which may be worth investigating at:
- git://github.com/jelera/vim-javascript-syntax.git
- git://github.com/pangloss/vim-javascript.git (seems to be the 'official' one now on http://www.vim.org/scripts/script.php?script_id=4452)

in order to add some jsdoc tags (interface, implements, typedef, todo).

Plugins to investigate:
- https://github.com/heavenshell/vim-jsdoc
- http://vimcasts.org/blog/2011/05/the-fugitive-series/
