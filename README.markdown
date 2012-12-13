## Intro
vimflowy is a vim plugin which implements a simple and elegant outliner tool like [workflowy](http://www.workflowy.com). It is based on [vimoutliner](http://www.github.com/vimoutliner/vimoutliner) and the document is still vimoutliner's.

## Features
- simple and elegent
- based on plain text file, you can open it everywhere and on every platform, with or without internet access.
- easy to navigate among items
- # and @ are highlighted just as in twitter and workflowy. They can be used as "context" in GTD
- complete tasks will be archived and append a time stamp
- extensible with other vim plugins (VOoM and universal text linking)

## Installation  
Using [pathogen](http://www.github.com/tpope/vim-pathogen) is strongly encouraged. 
		git submodule git://github.com/laoyang945/vimflowy.git .vim/bundle/vimflowy

## Usage
- Open a .otl file and the plugin will be automatically loaded
- In the insert mode, you can use TAB key to indent items to build a structured outliner.
- In the normal mode, you can use TAB key to expand/collapse the current line.
- If one line starts with colon(:) or semicolon (;), it will displayed as supplement text.
- You can use zs to filter out lines containing the word under the cursor and zn to show all lines
- Once a line is done, simply use ,,dn to archive this item (and all its descendants) to a sibling DONE node and append it's finishing time.

## Shortcut Key
- TAB: demote a heading in insert mode and expand/collapse nodes in normal mode
- ,,N(N=0~9): collapse to level N node, when N=0, collapse all
- zs: filter lines containing word under the cursor
- zn: equal to ,,0
- ,,dn: mark one line as done and append the time stamp
- ,,t: insert time
- ,,d: insert date

## Configration
- color scheme: Please modify colors/vo\_dar.vim
