<!-- Autor: Daniel Benjamin Perez Morales -->
<!-- GitHub: https://github.com/DanielPerezMoralesDev13 -->
<!-- Correo electrónico: danielperezdev@proton.me -->
# ***Guide to Neovim: Installation, Commands, Customization, Installing Extensions, and Creating Extensions***

> *Welcome to the comprehensive guide to Neovim, a highly configurable and extensible text editor. This guide will take you through the steps to install Neovim, familiarize yourself with its basic commands, customize it to your preferences, and create your own extensions.*

## ***Contents***

- [***Guide to Neovim: Installation, Commands, Customization, Installing Extensions, and Creating Extensions***](#guide-to-neovim-installation-commands-customization-installing-extensions-and-creating-extensions)
  - [***Contents***](#contents)
  - [***Installation of Neovim***](#installation-of-neovim)
  - [***Basic Neovim Commands***](#basic-neovim-commands)
  - [***Customization***](#customization)
  - [***Installing Extensions***](#installing-extensions)
  - [***Creating Extensions***](#creating-extensions)
  - [***Contributions***](#contributions)
  - [***License***](#license)

## ***Installation of Neovim***

*To install Neovim on your system, follow the specific instructions for your platform on the [official Neovim website](https://neovim.io/).*

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

## ***Basic Neovim Commands***

*Once you have installed Neovim, here are some basic commands to get you started:*

- **Open Neovim:**
  
  ```bash
  nvim
  ```

- **Exit Neovim:**
  
  *Press `Esc` to enter normal mode and then type `:q` followed by `Enter`.*

- **Save a File:**
  
  *In normal mode, type `:w` followed by `Enter`.*

- **Save and Quit:**
  
  *In normal mode, type `:wq` followed by `Enter`.*

## ***Customization***

> *Neovim is highly customizable. You can customize it by modifying the `init.vim` configuration file located at `~/.config/nvim/` on Unix systems. Here are some common settings you can add to your `init.vim` file:*

```vim
" Disable backup creation
set nobackup
set nowritebackup

" Enable syntax highlighting
syntax enable

" Set theme
colorscheme desert

" Adjust tab size to 4 spaces
set tabstop=4
set shiftwidth=4
set expandtab
```

## ***Installing Extensions***

*Neovim is highly extensible thanks to its extensive collection of extensions. You can install extensions using a package manager like [vim-plug](https://github.com/junegunn/vim-plug) or [Vundle](https://github.com/VundleVim/Vundle.vim). Here's an example of how to install a plugin using vim-plug:*

1. *Install vim-plug following the instructions on its repository.*
2. *Add desired plugins to your `init.vim` file:*

   ```vim
   call plug#begin('~/.vim/plugged')

   " Example Plugin
   Plug 'scrooloose/nerdtree'

   call plug#end()
   ```

3. *Save the file and reload the Neovim configuration by running:*

   ```bash
   :source ~/.config/nvim/init.vim
   ```

4. *Install the plugins by running:*

   ```bash
   :PlugInstall
   ```

## ***Creating Extensions***

*If you're interested in creating your own extensions for Neovim, you can find detailed documentation on the [official Neovim website](https://neovim.io/doc/user/).*

## ***Contributions***

*Contributions are welcome! If you have suggestions, corrections, or enhancements for this guide, feel free to open an issue or submit a pull request.*

## ***License***

*This repository is published under the MIT License. Feel free to use, modify, and distribute the content in accordance with the terms of this license.*
