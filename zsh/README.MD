## Installation

Install ZSH using Homebrew:
```bash
$ brew install zsh
```
Oh My Zsh
```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

chsh -s $(which zsh)
```
Configuration

To apply the changes you make you need to either start new shell instance or run:

```bash
$ source ~/.zshrc
```
Plugins
Add plugins to your shell by adding the name of the plugin to the plugin array in your .zshrc.

```bash
plugins=(git colored-man colorize pip python brew osx zsh-syntax-highlighting)
```
You'll find a list of all plugins on the Oh My Zsh Wiki. Note that adding plugins can cause your shell startup time to increase.

Themes
Changing theme is as simple as changing a string in your configuration file. The default theme is robbyrussell.
```
ZSH_THEME=pygmalion
```

[Oh My Zsh Wiki](https://github.com/robbyrussell/oh-my-zsh/wiki/themes)
