<!-- Autor: Daniel Benjamin Perez Morales -->
<!-- GitHub: https://github.com/DanielPerezMoralesDev13 -->
<!-- Correo electrónico: danielperezdev@proton.me -->
# ***Guía para Neovim: Instalación, Comandos, Personalización, Instalar Extensiones y Creación de Extensiones***

> *Bienvenido a la guía completa para Neovim, un editor de texto altamente configurable y extensible. Esta guía te llevará a través de los pasos para instalar Neovim, familiarizarte con sus comandos básicos, personalizarlo según tus preferencias y crear tus propias extensiones.*

## ***Contenido***

- [***Guía para Neovim: Instalación, Comandos, Personalización, Instalar Extensiones y Creación de Extensiones***](#guía-para-neovim-instalación-comandos-personalización-instalar-extensiones-y-creación-de-extensiones)
  - [***Contenido***](#contenido)
  - [***Instalación de Neovim***](#instalación-de-neovim)
  - [***Comandos Básicos de Neovim***](#comandos-básicos-de-neovim)
  - [***Personalización***](#personalización)
  - [***Instalación de Extensiones***](#instalación-de-extensiones)
  - [***Creación de Extensiones***](#creación-de-extensiones)
  - [***Contribuciones***](#contribuciones)
  - [***Licencia***](#licencia)

## ***Instalación de Neovim***

*Para instalar Neovim en tu sistema, sigue las instrucciones específicas para tu plataforma en el [sitio web oficial de Neovim](https://neovim.io/).*

- *Debian Ubuntu*

```bash
# Debian Ubuntu Install
sudo apt-get install nvim
```

- *Arch Linux*

```bash
# Arch Linux Install
sudo pacman -Syu nvim
```

## ***Comandos Básicos de Neovim***

*Una vez que hayas instalado Neovim, aquí hay algunos comandos básicos que te ayudarán a comenzar:*

- **Abrir Neovim:**
  
  ```bash
  nvim
  ```

- **Salir de Neovim:**
  
  *Presiona `Esc` para entrar en el modo normal y luego escribe `:q` seguido de `Enter`.*

- **Guardar un Archivo:**
  
  *En el modo normal, escribe `:w` seguido de `Enter`.*

- **Guardar y Salir:**
  
  *En el modo normal, escribe `:wq` seguido de `Enter`.*

## ***Personalización***

> *Neovim es altamente personalizable. Puedes personalizarlo modificando el archivo de configuración `init.vim` ubicado en `~/.config/nvim/` en sistemas Unix. Aquí hay algunas configuraciones comunes que puedes agregar a tu archivo `init.vim`:*

```vim
" Desactivar la creación de copias de seguridad
set nobackup
set nowritebackup

" Habilitar resaltado de sintaxis
syntax enable

" Establecer tema
colorscheme desert

" Ajustar el tamaño del tabulador a 4 espacios
set tabstop=4
set shiftwidth=4
set expandtab
```

## ***Instalación de Extensiones***

*Neovim es altamente extensible gracias a su amplia colección de extensiones. Puedes instalar extensiones utilizando un administrador de paquetes como [vim-plug](https://github.com/junegunn/vim-plug) o [Vundle](https://github.com/VundleVim/Vundle.vim). Aquí hay un ejemplo de cómo instalar un plugin utilizando vim-plug:*

1. *Instala vim-plug siguiendo las instrucciones en su repositorio.*
2. *Agrega los plugins deseados a tu archivo `init.vim`:*

   ```vim
   call plug#begin('~/.vim/plugged')

   " Plugin de ejemplo
   Plug 'scrooloose/nerdtree'

   call plug#end()
   ```

3. *Guarda el archivo y recarga la configuración de Neovim ejecutando:*

   ```bash
   :source ~/.config/nvim/init.vim
   ```

4. *Instala los plugins ejecutando:*

   ```bash
   :PlugInstall
   ```

## ***Creación de Extensiones***

*Si estás interesado en crear tus propias extensiones para Neovim, puedes encontrar documentación detallada en el [sitio web oficial de Neovim](https://neovim.io/doc/user/).*

## ***Contribuciones***

*¡Las contribuciones son bienvenidas! Si tienes sugerencias, correcciones o mejoras para esta guía, siéntete libre de abrir un problema o enviar una solicitud de extracción.*

## ***Licencia***

*Este repositorio se publica bajo la Licencia MIT. Siéntete libre de utilizar, modificar y distribuir el contenido de acuerdo con los términos de esta licencia.*
