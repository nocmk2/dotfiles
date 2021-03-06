aseom.dotfiles
==============

Here are some delightful dotfiles for my everyday use.

MacBook Pro
-----------

Disable requiring password after sleep.  
Disable "Disable automatic login" in the security preferences.  
Map `Cmd` + `Space` for selecting next input source.  
Install XCode and Homebrew.

```Shell
git clone --recursive https://github.com/aseom/dotfiles.git ~/dotfiles
cd ~/dotfiles && ./install.sh
```
Run `update.sh` for updating all submodules under the `vendor` directory.

#### Vim
```Shell
brew install vim --with-lua  # neocomplete requires lua
brew cask install macvim     # or install MacVim
vim +PlugInstall +qa         # Install plugins
```

#### Zsh
```Shell
brew install zsh

# As default shell
sudo cp -p /etc/shells /etc/shells.backup_
echo $(which zsh) | sudo tee -a /etc/shells
chpass -s $(which zsh)
```

Wiki
----

#### [Bookmarks & Cheatsheet](https://github.com/aseom/dotfiles/wiki)
