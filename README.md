# Dotfiles 

My personal dotfiles. 

## Repository 
A bare repository and a git alias is used to directly track dotfiles inside the
home directory without messing up other git repos. 

### Setup 
```sh
$ git init --bare ~/.dotfiles
$ alias dotgit='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'
$ dotgit config status.showUntrackedFiles no

```
### Checkout 
```sh
$ git clone --bare git@github.com:innerand/dotfiles.git $HOME/.dotfiles
$ alias dotgit='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'
$ dotgit checkout
```
Also see
https://wiki.archlinux.org/title/Dotfiles#Tracking_dotfiles_directly_with_Git
and https://www.atlassian.com/git/tutorials/dotfiles .


