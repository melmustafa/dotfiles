# Welcome to my dotfiles

Here are the configuration for the tooling I use daily. It includes [neovim](https://neovim.io) (code editor), [tmux](https://github.com/tmux/tmux/wiki) (terminal multiplexer), [zsh](https://www.zsh.org) (shell), [oh-my-zsh](https://ohmyz.sh) (zsh framework), [powerlevel10k](https://github.com/romkatv/powerlevel10k) (zsh theme), and [alacritty](https://alacritty.org) (terminal emulator).

## Zsh

Z-Shell or zsh is a configurable unix shell that provides powerful community-backed plugins.

### Zsh Installtion

- Ubuntu/Debian

  ```bash
  sudo apt install zsh
  ```

- Arch

  ```bash
  sudo pacman -Syu zsh
  ```

### Set Zsh as Default Shell

Add the following line at the top of `.bashrc`

```bash
exec zsh
```

If you ever want to remove zsh you should delete the added line.

## Oh-My-Zsh

Oh-My-Zsh is a zsh framework that manges themes, plugins, and configuration. It is well-maintained and documented with a wide arange of pre-installed plugins.

### Oh-My-Zsh Installation

Just run the following:

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

### Oh-My-Zsh Plugins

Oh-My-Zsh comes backed with a lot of useful plugins [built-in plugins](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins). I use some additional plugins as well.

Additional Plugins:

- [you-should-use](https://github.com/MichaelAquilina/zsh-you-should-use). This plugin will show you aliases you have set so that you can use them.
- [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions). This plugin suggest command completeion depending on your past commands usage.
- [zsh-bat](https://github.com/fdellwing/zsh-bat). This plugin will use `bat` instead of `cat` when ever `cat` is called. **`bat`** is the same as `cat` but is git and code aware. **You must install `bat` before hand**. I recommend installing it using `webi`.

  ```bash
  curl -sS https://webi.sh/bat | sh
  ```

- [zsh-lsd](https://github.com/z-shell/zsh-lsd). This plugin will use `lsd` instead of `ls` when ever `ls` is called. **`lsd`** is the same as `ls` with support for better and cleaner font and coloring. **You must install `lsd` before hand**. I recommend installing it using `webi`.

  ```bash
  curl -sS https://webi.sh/lsd | sh
  ```

- [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting). This plugin provide highlighting in the terminal so you know what is a command and what is just an argument.

You will need `git` to install most of Oh-My-Zsh related configuration and plugins so I advise you to install `git` first.

To install git:

- Ubuntu/Debian

  ```bash
  sudo apt install git
  ```

- Arch

  ```bash
  sudo pacman -Syu git
  ```
