# Path to your oh-my-zsh installation.
export ZSH="$HOME/.config/zsh/.oh-my-zsh"

#Theme for the zsh-shell
ZSH_THEME="gallois"

# Built-In Plugins
plugins=(git)

# Load oh-my-zsh shell integration
source $ZSH/oh-my-zsh.sh

# Load antigen source file
source /opt/homebrew/Cellar/antigen/2.2.3/share/antigen/antigen.zsh

# Load the oh-my-zsh library
antigen use oh-my-zsh

#antigen bundles
antigen bundle z # improved the file movement
antigen bundle colored-man-pages

# zsh-users antigen bundles
antigen bundle zsh-users/zsh-syntax-highlighting
antigen bundle zsh-users/zsh-autosuggestions
antigen bundle zsh-users/zsh-completions

# Apply bundle changes
antigen apply

# Aliase
alias zconf="vim ~/.config/zsh/.zshrc"
alias zsource="source ~/.config/zsh/.zshrc"
alias vim="nvim"