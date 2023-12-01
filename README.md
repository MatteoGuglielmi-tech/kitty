## 📖 Table of Contents 📖

<!--toc:start-->

- [❓ What are we talking about? ❓](#what-are-we-talking-about)
- [🔧 How to set a color scheme 🔧](#🔧-how-to-set-a-color-scheme-🔧)
  - [📁 Color schemes palette 📁](#📁-color-schemes-palette-📁)
  - [⬇️ Installation ⬇️](#️-installation-️)
  - [⚠️ Disclaimer ⚠️](#️-disclaimer-️)
  <!--toc:end-->

## 🎨 Author 🎨

Author/Owner : Guglielmi Matteo [@GitHub](https://github.com/MatteoGuglielmi-tech)

## ❓ What are we talking about? ❓

This repository contains a <b><u>personal configuration</u></b> for [kitty](https://sw.kovidgoyal.net/kitty/), a terminal emulator for Linux, macOS and Windows.  
The core settings for kitty are in the `kitty.conf` file, while the `theme.conf` file contains the color scheme for the terminal.
To set an arbitrary color scheme, please refer to [this](#🔧-how-to-set-a-color-scheme-🔧).

## 🔧 How to set a color scheme 🔧

In the following, a concise guide to set an available color scheme for kitty is provided along with a collection of themes I used.

### 📁 Color schemes palette 📁

> Personalize your kitty terminal and choose your theme from this awesome collection [...]

The source GitHub repo is provided by [dexpota](https://github.com/dexpota) and can be found [here](https://github.com/dexpota/kitty-themes?search=1). In the latter, you can find a graphical representation of the color palettes associated to every color scheme alongside a detailed description on how to set the different themes. Despite that, if you're looking for a shorter "tutorial", follow along.

### ⬇️ Installation ⬇️

1. Clone `kitty-themes` in your kitty configuration folder (usually `~/.config/kitty/`):

```bash
git clone --depth 1 https://github.com/dexpota/kitty-themes.git ~/.config/kitty/kitty-themes
```

2. Link the config file corresponding to the theme you want to use to `~/.config/kitty/theme.conf`:

```bash
cd ~/.config/kitty/ && ln -s ~/.config/kitty/kitty-themes/themes/<THEMENAME>.conf ~/.config/kitty/theme.conf
```

3. Inform kitty about the new theme by adding the following line to your `kitty.conf`:

```bash
include ./theme.conf
```

4. Restart kitty and enjoy your new theme!

### ⚠️ Disclaimer ⚠️

This set-up has been tested only on <u>macOS and Arch Linux machines</u>. If you're using Windows, please refer to the official [kitty documentation](https://sw.kovidgoyal.net/kitty/conf.html) for further information and to [kitty-themes documentation](https://github.com/dexpota/kitty-themes?search=1).
