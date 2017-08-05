# Molokai Color Scheme for Vim, with transparent terminal backgrounds

Molokai is a Vim port of the monokai theme for TextMate originally created by Wimer Hazenberg.

This fork adds `molokai-term`, a modified version of Molokai that looks better on 256-color terminals and has no background of its own, so it looks good with transparent (but dark!) terminals. Made possible with [CSApprox](https://github.com/godlygeek/csapprox) by Matt Wozniski and the original [molokai](https://github.com/tomasr) by Tomas Restrepo.

By default, it has a dark gray background based on the version created by Hamish Stuart Macpherson for the E editor.

![Gray Background](http://www.winterdom.com/weblog/content/binary/WindowsLiveWriter/MolokaiforVim_8602/molokai_normal_small_3.png)

![Molokai Original](http://www.winterdom.com/weblog/content/binary/WindowsLiveWriter/MolokaiforVim_8602/molokai_original_small_3.png)


## Installation and Usage

Copy the files to your .vim/colors folder, or use Vundle/Pathogen/your favorite
Vim plugin manager. Then use the following code in your `.vimrc`
(`molokai_original` setting optional):

```vim
set background=dark

if has("gui_running")
    let g:molokai_original = 1
    colorscheme molokai
else
    colorscheme molokai-term
endif
```
