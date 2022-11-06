## Windows
  - [Visual Studio Code](https://code.visualstudio.com/download)
  - [Git](https://git-scm.com/downloads) - [*Config*](https://git-scm.com/book/pt-br/v2/Começando-Configuração-Inicial-do-Git)
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

## WSL - Docker

    # Install
    sudo apt update && sudo apt upgrade
    sudo apt remove docker docker-engine docker.io containerd runc
    sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg \
    lsb-release
    
    # Add Docker repo in sources - Ubuntu
    curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
    echo \
      "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
      $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
      
    # Install Docker-Engine
    sudo apt-get update
    sudo apt-get install docker-ce docker-ce-cli containerd.io docker-compose-plugin
    
    # Permission
    sudo usermod -aG docker $USER
    
    # Service Docker
    sudo service docker start
    
    # Windows 11
    sudo vim /etc/wsl.conf
    > [boot]
    > command="service docker start" 
