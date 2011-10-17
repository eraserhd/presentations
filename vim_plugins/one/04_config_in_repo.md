!SLIDE bullet incremental
# Sharing Vim Configs #

* Dropbox
* Git

!SLIDE bullet incremental
# Dropbox #

* Simple to set up
* Not good for pairing
* Hard for multiple archs

!SLIDE bullet incremental
# Git #

* Harder to set up
* Works for pairing
* Works for multiple archs

!SLIDE bullet incremental
# Setup #

* mkdir ~/Dropbox/Vim
* mv ~/.vimrc ~/Dropbox/Vim/vimrc
* mv ~/.vim ~/Dropbox/Vim/vimfiles

!SLIDE
# Change vimrc #

    @@@ Vim
    let &runtimepath =
      \ expand("<sfile>:p:h") .
      \ "/vimfiles," .
      \ &runtimepath
    call pathogen#infect()

!SLIDE bullet incremental
# With Git #

* git clone --recursive foo:/bar/my_stuff.git
* echo 'source ~/my_stuff/vimrc' >~/.vimrc

