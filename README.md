# settings
My Development Environment Settings

# Brew

## Install Brew
```zsh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## Run `brew bundle` with `~/Brewfile`
```zsh
brew bundle
```

# ZSH

## Install Oh My Zsh & Plugins
```zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

## Download `~/.p10k.zsh` or Run `p10k configure`
> `powerlevel10k/p10k` already installed with `brew bundle`

If You don't want to download it, Do configure
```zsh
p10k configure
```

## Download `~/.zshrc`
