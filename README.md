## Windows
  - [Choco](https://www.liquidweb.com/kb/how-to-install-chocolatey-on-windows/)
  - [Visual Studio Code](https://code.visualstudio.com/download)
  - [Git](https://git-scm.com/downloads) - [*Config*](https://git-scm.com/book/pt-br/v2/Começando-Configuração-Inicial-do-Git) - [*SSH*](https://docs.github.com/pt/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent?platform=linux)
  - [Font Powerline](https://gist.github.com/stramel/658d702f3af8a86a6fe8b588720e0e23)
  - [Inter](https://fonts.google.com/specimen/Inter)
  - [JetBrains Mono](https://www.jetbrains.com/pt-br/lp/mono/)

<br />

## WLS 2
    
*Install Distro*

```bash
wsl --install -d distro
```

*Uninstall Distro*

```bash
wsl --unregister -d distro
```
    
*Config file*

```bash
touch C:\Users\<username>\.wslconfig
```

```bash
vim C:\Users\<username>\.wslconfig
```

```txt
[wsl2]
memory=8GB
processors=4
swap=2GB
```

<br />

### Zsh

*Install*

```bash
sudo apt install zsh
```

*Defaullt Shell*

```bash
chsh -s /usr/bin/zsh
```

*Close Terminal and open again (option 2)*

<br />

### Oh My Zsh
    
*Install*

```bash
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
    
#### Plugins: 
  - [F-Sy-H](https://github.com/zdharma/fast-syntax-highlighting)
  - [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions)
  - [zsh-completions](https://github.com/zsh-users/zsh-completions)

#### Theme:
  - [powerlevel10k](https://github.com/romkatv/powerlevel10k)

<br />

*Config*

```bash
code ~/.zshrc
```

```txt
[zshrc]

ZSH_THEME="powerlevel10k/powerlevel10k"

plugins=(git git-flow F-Sy-H zsh-autosuggestions zsh-completions)
```
    
```bash
source ~/.zshrc
```

```bash
#Reset Config
p10k configure
```

<br />

### Ansible

```bash
sudo apt update
sudo apt install software-properties-common
sudo add-apt-repository --yes --update ppa:ansible/ansible
sudo apt install ansible
```

```bash
sudo ansible-playbook -i localhost, -c local playbook.yml --extra-vars "user_name=your_username"
```

*Execute with o file `playbook.yml` in repository*
