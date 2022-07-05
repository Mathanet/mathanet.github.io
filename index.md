# The first step when you install Ubuntu

## Connect to Github Quickly in China

- [Github520](https://gitee.com/inChoong/GitHub520)
- [Steam++(Recommend)](https://steampp.net)

  - Usage

    To use `curl` or `wget`, run the following commands

    ```bash
    # Copy the certificate to `/usr/local/share/ca-certificates`
    # Note: It is important to have the .crt extension on the file, otherwise it will not be processed.
    # The certificate may be use .cer extension, just revise it as .crt

    sudo cp certificate.crt /usr/local/share/ca-certificates
    sudo update-ca-certificates
    ```

 Now you can connect to Github steadily

---

## Terminal

use zsh and [oh-my-zsh](https://github.com/ohmyzsh/ohmyzsh)

### Installation

1. Install zsh

    ```bash
    sudo apt install zsh
    ```

2. Install oh-my-zsh

	| Method | Command |
	| - | - |
	| curl | `sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"` |
	| wget | `sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"` |
	| fetch | `sh -c "$(fetch -o - https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"` |

### Config

- [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions)

  - Installation

    1. Clone the repository into `$ZSH_CUSTOM/plugins` (by default `~/.oh-my-zsh/custom/plugins`)

        ```sh
        git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
        ```

    2. Add the plugin to the list of plugins for Oh My Zsh to load (inside `~/.zshrc`):

        ```bash
        plugins=( 
            # other plugins...
            zsh-autosuggestions
        )
        ```

    3. Start a new terminal session.

- [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)

  - Installation

    - Clone the repository in oh-my-zsh's plugins directory:

    ```zsh
    git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
    ```

    - Activate the plugin in `~/.zshrc`:

    ```zsh
    plugins=( [plugins...] zsh-syntax-highlighting)
    ```

    - Restart zsh (such as by opening a new instance of your terminal emulator).

## Applications

- [etcher](https://www.balena.io/etcher/)
- [WoeUSB](http://download.opensuse.org/repositories/home:/Provessor/xUbuntu_20.04/amd64/)
- [chrome](https://www.google.cn/chrome/index.html)
- [vscode](https://code.visualstudio.com/)
- [edge](https://www.microsoft.com/zh-cn/edge)
- [nvim](https://github.com/neovim/neovim)
- [icalingua++ (QQ for linux)](https://github.com/icalingua-plus-plus/icalingua-plus-plus)

---

## fonts

### How to install fonts in Ubuntu?

Unpack fonts to `~/.local/share/fonts` (or `/usr/share/fonts`, to install fonts system-wide) and `fc-cache -f -v`

or add them in `/etc/fonts/conf.d/64-language-selector-prefer.conf`

here is some recommend

---
Chinese fonts(open source)

- [LXGW WenKai](https://github.com/lxgw/LxgwWenKai)
- [LXGW WenKai Screen](https://github.com/lxgw/LxgwWenKai-Screen)
- [LXGW New Clear Gothic](https://github.com/lxgw/LxgwNewClearGothic)

And these fonts' [release](http://lxgw.ysepan.com/)

English fonts

- [JetBrainsMono Nerd Font](https://www.nerdfonts.com/font-downloads)

---

## Input

use [rime](https://rime.im), and here is rime's [wiki](https://github.com/rime/home/wiki)

### Install

```bash
sudo apt install ibus-rime

# wubi
sudo apt install librime-data-wubi

```

<https://blog.csdn.net/Sacredness/article/details/92195032>

---
