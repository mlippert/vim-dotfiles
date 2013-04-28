
vim-dotfiles
============

My configuration files for vim.

## Manual config ##

A few things may need to be done the first time these dot files
are installed to make sure vim finds them and doesn't have any issues.

Create links

- `.vimrc` -> `.vim/rc/vimrc`
- `.gvimrc` -> `.vim/rc/gvimrc`

Make sure that the directory `.vim/tmp` exists for storing backup files

## Notes on the vim configuration ##

uses pathogen to install plugins located in `.vim/bundle`
Those plugins are submodules
- supertab
- vim-colors-solarized
- vim-jsbeautify

I have edited the .vim/javascript.vim file I originally got from:
http://vadconf.googlecode.com/svn/trunk/vim/syntax/javascript.vim  
in order to add some jsdoc tags (interface, implements, typedef, todo).




## Future investigation ##

### Plugins ###
- [vim-jsdoc plugin][vim-jsdoc]
- [fugitive article][fugitive]
- [vim-markdown plugin][vim-markdown]

### syntax files ###
- git://github.com/jelera/vim-javascript-syntax.git
- git://github.com/pangloss/vim-javascript.git
  (seems to be the 'official' one now on http://www.vim.org/scripts/script.php?script_id=4452)

### color schemes ###

<!-- reference links section -->
[vim-jsdoc]: <https://github.com/heavenshell/vim-jsdoc> "vim-jsdoc plugin on github"
[fugitive]: <http://vimcasts.org/blog/2011/05/the-fugitive-series/> "article on vim fugitive plugin"
[vim-markdown]: <https://github.com/plasticboy/vim-markdown> "vim-markdown plugin by plasticboy on github"
