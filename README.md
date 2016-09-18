# Setup OS X work station from scratch

> List of configurations and tools that need to be added/installed in order to develop on the OS X machine with comfort (VERY OPIONATED).

<img src="https://media.giphy.com/media/mYtiMk3wqzNwQ/giphy.gif" />

- [x] [homebrew](http://brew.sh)
- [x] [homebrew-cask](https://caskroom.github.io)
- [x] [iterm2](https://www.iterm2.com)
- [x] [zsh](http://www.zsh.org)
- [x] [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)
- [x] [git](https://git-scm.com)
- [x] [tj/git-extras](https://github.com/tj/git-extras)
- [x] [vagrant](https://www.vagrantup.com)
- [x] [virtualbox](https://www.virtualbox.org)
- [x] browsers (chrome, chrome canary, firefox)
- [x] misc (spotify, dropbox, telegram, skype, vlc, evernote, etc.)
- [x] [commonly used aliases](https://github.com/voronianski/setup-osx-work-station/blob/master/scripts/aliases.sh#L2-L13)

## Configs

### Oh My Zsh

##### .zshrc

```bash
# Path to your oh-my-zsh installation.
export ZSH=/Users/iunna/.oh-my-zsh

# Set name of the theme to load.
# Look in ~/.oh-my-zsh/themes/
# Optionally, if you set this to "random", it'll load a random theme each
# time that oh-my-zsh is loaded.
ZSH_THEME="agnoster"

CASE_SENSITIVE="true"

# Which plugins would you like to load? (plugins can be found in ~/.oh-my-zsh/plugins/*)
# Custom plugins may be added to ~/.oh-my-zsh/custom/plugins/
# Example format: plugins=(rails git textmate ruby lighthouse)
# Add wisely, as too many plugins slow down shell startup.
plugins=(git zsh-autosuggestions encode64)

source $ZSH/oh-my-zsh.sh

# get all aliases
source ~/.shrc

# Preferred editor for local and remote sessions
export EDITOR='vi'
```

### iTerm 2

##### Enable word jumps

By default, word jumps (`options + →` or `options + ←`) do not work. To make them work go to `iTerm -> Preferences -> Keys` and add following shortcuts:

_Option + right_

```
⌥→
Send Escape Sequence
f
```

_Option + left_

```
⌥←
Send Escape Sequence
b
```

---

**MIT Licensed**
