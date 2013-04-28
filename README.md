
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

uses pathogen to install plugins located in `.vim/bundle`.
These plugins are git submodules.

- [supertab][]
- [vim-colors-solarized][solarized]
- [vim-jsbeautify][jsbeautify]

I have edited the `.vim/javascript.vim` file I originally got from
<http://vadconf.googlecode.com/svn/trunk/vim/syntax/javascript.vim>
in order to add some jsdoc tags (interface, implements, typedef, todo).

Uses the solarized color scheme with a few minor adjustments in `.gvimrc`.

I've put a bunch of color schemes into the `.vim/colors` directory, including one named *lippert* that I created using [vivify][], but I ended up not loving any of them and realizing that all I needed was a couple of adjustments I could make in `.gvimrc`.

## Future investigation ##

### Plugins ###
- [vim-jsdoc plugin][vim-jsdoc]
- [fugitive article][fugitive]
- [vim-markdown plugin][vim-markdown]

### syntax files ###
- [vim-javascript][js-syntax-j] by jelera
- [vim-javascript][js-syntax-pg] by pangloss
  (seems to be the 'official' one now on [vim.org][vimorg-4452])

### color schemes ###



[supertab]: <https://github.com/ervandew/supertab> "supertab plugin on github"
[solarized]: <https://github.com/altercation/vim-colors-solarized> "solarized plugin on github"
[jsbeautify]: <https://github.com/maksimr/vim-jsbeautify> "vim-jsbeautify plugin on github"
[vim-jsdoc]: <https://github.com/heavenshell/vim-jsdoc> "vim-jsdoc plugin on github"
[fugitive]: <http://vimcasts.org/blog/2011/05/the-fugitive-series/> "article on vim fugitive plugin"
[vim-markdown]: <https://github.com/plasticboy/vim-markdown> "vim-markdown plugin by plasticboy on github"
[js-syntax-j]: <https://github.com/jelera/vim-javascript-syntax> "jelera's javascript syntax file on github"
[js-syntax-pg]: <https://github.com/pangloss> "pangloss's javascript syntax file on github"
[vimorg-4452]: <http://www.vim.org/scripts/script.php?script_id=4452> "vim.org javascript syntax file"
[vivify]: <http://bytefluent.com/vivify/> "web tool to create vim color schemes"
