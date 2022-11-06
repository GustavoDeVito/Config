## Windows
  - [Font Powerline](https://gist.github.com/stramel/658d702f3af8a86a6fe8b588720e0e23)

## WLS 2
    
    # Install Distro
    wsl --install distro

    # Uninstall Distro
    wsl --unregister distro
    
    # Config file > C:\Users\<username>\.wslconfig
    [wsl2]
    memory=12GB
    processos=4
    swap=4GB


## WSL 2 - Ubuntu
  
    sudo apt update
    sudo apt install curl wget git
  
    # Zsh
    # Install
    sudo apt install zsh

    # Defaullt Shell
    chsh -s /usr/bin/zsh

    # Close Terminal and open again (option 2).

    # oh-my-zsh
    # Install
    sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
    
    # Install Plugins
    # Intall Theme

    code ~/.zshrc
    > ZSH_THEME="powerlevel10k/powerlevel10k"
    > plugins=(git git-flow F-Sy-H zsh-autosuggestions zsh-completions)
    source ~/.zshrc

#### Plugins: 
  - [F-Sy-H](https://github.com/zdharma/fast-syntax-highlighting)
  - [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions)
  - [zsh-completions](https://github.com/zsh-users/zsh-completions)
 
#### Theme:
  - [powerlevel10k](https://github.com/romkatv/powerlevel10k)
