# dotfile
linux conf files for better dev navigation.

## Configuration files
* bash
* vim
* tmux

```shell
sudo apt-get install vim
sudo apt-get install tmux
```

**IMPORTANT:** Before changing any configurations make sure you backup the original config files.

## Bash Configuration
```shell
cp bashrc ~/.bashrc
```
**IMPORTANT:** Make sure you do not put any key inside bashrc file while pushing to the repo.

## Vim Configuration
```shell
cp vimrc ~/.vimrc
```
use [Vundle](https://github.com/VundleVim/Vundle.vim) for vim package management.
```shell
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```
To install Plugin run ```vim``` and execute ```:PluginInstall``` or run from command-line
``` vim +PluginInstall```

## Tmux Configuration
```shell
cp tmux.conf ~/.tmux.conf
tmux kill-server # kill and restart the server or
tmux source-file ~/.tmux.conf # reload the conf file in same session
```
