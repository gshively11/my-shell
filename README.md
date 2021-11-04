# my-shell

Installation and configuration for my shell.

## Initial Setup

I'm not sure if these step are idempotent, only run this once for initial setup.

Install Brew

```sh
# Set ZSH as default shell
chsh -s /bin/zsh

# Close and re-open terminal

# Install Brew
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# Install iTerm2
brew install --cask iterm2

# Close and open iTerm2

# Install zsh 
brew install zsh

# Close and open shell

# Install oh-my-zsh
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

# Install p10k theme
brew install romkatv/powerlevel10k/powerlevel10k

# Close and open shell, should enter p10k configuration
# Select prompt to install Meslo Nerd Font
# Quit iTerm2
# Ensure that iTerm2 is using Meslo font
# Open iTerm2

# Link dotfiles to home dir 
ln -s ~/my-shell/zshrc ~/.zshrc
ln -s ~/my-shell/p10k.zsh ~/.p10k.zsh

# Import my_shell.json as an iTerm2 Profile via GUI
```

## Cheatsheet

```sh
# Upgrade all brew installs
brew upgrade

# copy file to clipboard 
copyfile path/file.txt

# copy current directory to clipboard
copydir

# ctrl+o to copy current shell cmd buffer to clipboard
```
