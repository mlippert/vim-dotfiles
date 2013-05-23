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
These plugins are git submodules as recommended on [Vim Cast #27][submodules].

- [supertab][]
- [vim-colors-solarized][solarized]
- [vim-jsbeautify][jsbeautify]
- [taglist][]
- [LustyJuggler][lustyjuggler] : it's been recommended to use buffers w/ a plugin like this one rather than tabs.
- [NERDTree][]
- [vim-session][]
- [surround][] : This [article][surround-article describes it.
- [Ultisnips][] : the original snipmate author Marc Weber [recommends][snipmate-ultisnips] this snippet plugin now.

I have edited the `.vim/javascript.vim` file I originally got from
<http://vadconf.googlecode.com/svn/trunk/vim/syntax/javascript.vim>
in order to add some jsdoc tags (interface, implements, typedef, todo).

Uses the solarized color scheme with a few minor adjustments in `.gvimrc`.

I've put a bunch of color schemes into the `.vim/colors` directory, including one named *lippert* that I created using [vivify][], but I ended up not loving any of them and realizing that all I needed was a couple of adjustments I could make in `.gvimrc`.

### Key mappings ###

#### Command mode ####
- &lt;F8> - toggle the taglist window
- cp{motion} - Change by putting whats in the default("") yank buffer.
- &lt;leader>d - :NERDTreeToggle (File explorer)
- &lt;F12> - :LustyJuggler (open buffer list)

## Future investigation ##

### Plugins ###
- [vim-jsdoc plugin][vim-jsdoc]
- [fugitive article][fugitive] : I've read the article, and for now anyway, I don't think I need this plugin.
- [vim-markdown plugin][vim-markdown]

### syntax files ###
- [vim-javascript][js-syntax-j] by jelera
- [vim-javascript][js-syntax-pg] by pangloss
  (seems to be the 'official' one now on [vim.org][vimorg-4452])

### color schemes ###

### other people's vim configurations ###
[The perfect .vimrc vim config file][spf13] last updated May 2011


## Installation Notes ##

### MS Windows ###
Vim 7.3 for MS Windows has issues w/ ruby plugins, namely they crash gvim. Googling turned up others describing this problem as well as someone who has kindly recompiled vim for windows so it works and posted it. Thank you [Wu Yongwei](http://wyw.dcweb.cn/). The version I downloaded May 2013 worked like a charm.

[supertab]: <https://github.com/ervandew/supertab> "supertab plugin on github"
[solarized]: <https://github.com/altercation/vim-colors-solarized> "solarized plugin on github"
[jsbeautify]: <https://github.com/maksimr/vim-jsbeautify> "vim-jsbeautify plugin on github"
[vim-jsdoc]: <https://github.com/heavenshell/vim-jsdoc> "vim-jsdoc plugin on github"
[fugitive]: <http://vimcasts.org/blog/2011/05/the-fugitive-series/> "article on vim fugitive plugin"
[vim-markdown]: <https://github.com/plasticboy/vim-markdown> "vim-markdown plugin by plasticboy on github"
[js-syntax-j]: <https://github.com/jelera/vim-javascript-syntax> "jelera's javascript syntax file on github"
[js-syntax-pg]: <https://github.com/pangloss> "pangloss's javascript syntax file on github"
[vimorg-4452]: <http://www.vim.org/scripts/script.php?script_id=4452> "vim.org javascript syntax file"
[vim-session]: <https://github.com/xolox/vim-session> "vim-session on github"
[taglist]: <http://vim-taglist.sourceforge.net/> "tag-list plugin on sourceforge"
[lustyjuggler]: <https://github.com/vim-scripts/LustyJuggler> "lustyjuggler plugin on github"
[vivify]: <http://bytefluent.com/vivify/> "web tool to create vim color schemes"
[spf13]: <http://spf13.com/post/perfect-vimrc-vim-config-file> "Article on Steve Francia's blog about his vimrc"
[NERDTree]: <https://github.com/scrooloose/nerdtree> "NERDTree plugin on github"
[surround]: <https://github.com/tpope/vim-surround> "surround plugin on github"
[surround-article]: <http://www.catonmat.net/blog/vim-plugins-surround-vim/> "Peteris Krumins' blog article on the surround plugin"
[ultisnips]: <https://github.com/SirVer/ultisnips> "Ultisnips plugin mirror on github"
[snipmate-ultisnips]: <https://groups.google.com/forum/?fromgroups#!topic/vim_use/1-JNVqgNr5s> "Marc Weber comments on moving to Ultisnips"
[submodules]: <http://vimcasts.org/episodes/synchronizing-plugins-with-git-submodules-and-pathogen/> "Synchronizing plugins with git submodules and pathogen"

