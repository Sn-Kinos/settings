# Dev. Environment Settings on RHEL

## Initialize Environment
### DNF & Package Settings
```bash
sudo dnf update
sudo dnf install https://dl.fedoraproject.org/pub/epel/epel-release-latest-8.noarch.rpm
sudo dnf update
```

### Install Requirements
```
sudo dnf install zsh autojump-zsh neovim git python3-devel gcc
```

## ZSH Settings

### Install Oh My Zsh & Powerlevel10k & fzf
```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf && ~/.fzf/install
```

### Install ZSH Plugins
```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

### Install thefuck
```bash
pip3 install thefuck --user
```

### Set ZSH to default shell
```zsh
sudo chsh $USER
/bin/zsh
```
### Use `.zshrc` on this folder
1. Enter (q) on zsh initializing menu.
2. Copy and paste `.zshrc` on this folder
3. Rerun `zsh`

