# Custom-Terminal-Theme

Customize your terminal (Oh My Zsh) on Ubuntu

![Screenshot](img/screenshot.png)

## Update the packages

```
  sudo apt-get update
  sudo apt upgrade
```

## Install prerequisite packages (ZSH, powerline & powerline fonts)

```
 sudo apt install zsh
 sudo apt-get install powerline fonts-powerline
```

## Clone the Oh My Zsh Repo

```
 git clone https://github.com/robbyrussell/oh-my-zsh.git ~/.oh-my-zsh
```

## Create a New ZSH configuration file

```
 cp ~/.oh-my-zsh/templates/zshrc.zsh-template ~/.zshrc
```

## Install PowerLevel10k!

```
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```

## Set up a theme for your Terminal — Open .zshrc File using gedit editor

```
 nano ~/.zshrc
```

## And change and put these lines :

```
 ZSH_THEME="powerlevel10k/powerlevel10k"
```

## Change your Default Shell

```
 chsh -s /bin/zsh
```

# Install some plugins

## ZSH Syntax Highlighting

```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

## ZSH Autosuggestions

```
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

## Open zsh file and enable your new plugins

```
sudo nano ~/.zshrc
```

```
plugins=( git
 zsh-syntax-highlighting
 zsh-autosuggestions)
```




# Finally restart your promp to set the new features