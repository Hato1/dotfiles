# Dotfiles

This is my configuration. There are many like it, but this one is mine.



## Version history & TODO

0.1: Last tested in Linux Mint 20.3 Cinnamon.

TODO: Add commandline tool Cheat & my cheatfiles.

## CLI Installs

```
apt install openssh-server
apt install zsh  # Pre-requisite for oh-my-zsh
apt install gtimelog
apt install git
apt install spotify-client
apt install sublime-text
apt install silversearcher-ag
apt install python3-distutils  # Poetry requirement
apt install mailutils  # Local. Cron job stderr emails here.
```



## Manual installs

* [Install Pycharm Toolbox](https://www.jetbrains.com/toolbox-app/) and use it to install Pycharm community edition.
* [Install PyPoetry](https://python-poetry.org/docs/) and add to PATH.
* [Install Obsidian](https://obsidian.md/download)
* [Install GitKraken](https://www.gitkraken.com/download)
* [Install Typora](https://support.typora.io/Typora-on-Linux/)
* [Install oh my zsh](https://ohmyz.sh/#install)



## Mouse button configuration
Useful for customising extra mouse buttons

Use version 1.5.1 if using Ubuntu 22.04 or earlier.

* [Install input-remapper](https://github.com/sezanzeb/input-remapper/releases)

```yaml
Wheel Left: KEY_PREVIOUSSONG
Wheel Right: KEY_NEXTSONG
Side button: Ctrl + Alt + Left (Previous workspace)
Side button 2: Ctrl + Alt + Right (Next workspace)
```



## Desktop

Install Mojave wallpaper.
`gsettings set org.gnome.desktop.background picture-uri "file:/home/jacob/Software/dotfiles/wallpapers/mojave.xml"`



## SSH

* Install ssh keys
* Disable password authentication & PAM.



## Terminal

1. Set terminal preferences like images in `terminal/terminal-*.png`.
2. `cp terminal/doubleend.zsh-theme ~/.oh-my-zsh/themes`
3. `cp terminal/zshrc ~/.zshrc`
4. Restart to have ZSH be the default shell. Relogging isn't always sufficient.



## Sublime Text

Copy contents of `Preferences.sublime.settings` into the sublime settings file by the same name.



## Pycharm

Import settings by either importing them from `pycharm/settings.zip` or by utilising jetbrains cloud settings sync.



## Dracula Themes
Install [Dracula theme](https://draculatheme.com/) for Slack & Obsidian & Typora, etc
