# Instalar Oh My ZSH

* Instalar zsh y git
  * sudo apt install git zsh
* Poner ZSH como shell por defecto
  * chsh -s $(which zsh)
  * Cerrar sesión y volver a entrar.
* Instalar Oh My ZSH
  * sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

# Cambiar tema
  
* Tema honukai descargar
  * wget https://raw.githubusercontent.com/oskarkrawczyk/honukai-iterm/master/honukai.zsh-theme $ZSH_CUSTOM/themes/
  * Mover si es necesario dentro del directorio de temas
  * mv honukai.zsh-theme /home/"usuario"/.oh-my-zsh/themes/honukai.zsh-theme 
* Para activarlo hay que modificar el fichero de configuración ~/.zshrc:
  * ZSH_THEME="honukai"
  
 # Plugins
 
 * Para activarlos hay que modificar el fichero de configuración ~/.zshrc:
   * plugins=(
    git common-aliases colored-man-pages zsh-autosuggestions zsh-syntax-highlighting
    )
  
* Algunos plugins, además de activarlos hay que instalarlos.

* Plugin zsh-autosuggestions
  * Este plugin busca en el historial tus últimos comandos y te va autocompletando los mismos.
  * Para instalarlo: git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions

* Plugin zsh-syntax-highlighting
  * Este plugin colorea los comandos en verde o en rojo dependiendo de si son correctos o no.
  * Para instalarlo: git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting
  
