# 🖥️ p10k-config

This repository contains my customized [Powerlevel10k](https://github.com/romkatv/powerlevel10k) Zsh theme configuration, designed for a modern terminal experience with features like OS icons, date and time on separate lines, transparency-friendly colors, and a minimalist clean layout.

> ⚡ Optimized for Kali Linux (WSL), but works across all Linux distros.

---

## 📸 Preview

*Coming soon – add a screenshot to show off your prompt!*

---

## 📦 Dependencies

Before using this config, install the following:

### 1. Zsh

```bash
sudo apt update
sudo apt install zsh -y
```

Set Zsh as your default shell:

```bash
chsh -s $(which zsh)
```

Logout and log back in to apply.

---

### 2. Oh My Zsh

Install [Oh My Zsh](https://ohmyz.sh/) with this command:

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

---

### 3. Powerlevel10k

Clone the Powerlevel10k theme into the correct directory:

```bash
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git \
  ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```

Then edit your `~/.zshrc` to use the theme:

```bash
ZSH_THEME="powerlevel10k/powerlevel10k"
```

---

## 🚀 Installation (This Configuration)

### 1. Clone the Config

```bash
git clone https://github.com/Robel-S-Y/p10k-config.git
cd p10k-config
```

### 2. Copy the Config File

```bash
cp p10k.zsh ~/.p10k.zsh
```

### 3. Source the Config in `.zshrc`

Ensure your `~/.zshrc` contains this line:

```bash
[[ -f ~/.p10k.zsh ]] && source ~/.p10k.zsh
```

If not, add it manually at the end of the file.

---

### 4. Reload Zsh

Apply the changes by restarting your terminal or running:

```bash
source ~/.zshrc
```

---

## 🔧 Features & Customizations

✅ **Date + Time stacked vertically**, centered
✅ **Kali OS icon** (🐉) with dynamic username & hostname
✅ **Transparent background–friendly** prompt colors
✅ **Multiline prompt layout** for better readability
✅ Clean, minimal prompt with modern unicode lines

---

## 🧪 Tested On

* ✅ Kali Linux (WSL and native)
* ✅ Ubuntu
* ✅ Arch-based systems
* ✅ Any system running Zsh + Powerlevel10k

---

## 🧩 Optional: Nerd Fonts

For icons and symbols to render correctly, install a [Nerd Font](https://www.nerdfonts.com/):

```bash
# Example: Hack Nerd Font
wget https://github.com/ryanoasis/nerd-fonts/releases/latest/download/Hack.zip
unzip Hack.zip -d ~/.fonts
fc-cache -fv
```

Then configure your terminal to use the new font.

---

## 🧠 Tip: Backup or Sync

You can reuse this config on other machines by cloning this repo and repeating the install steps. If you want to sync changes across machines, use Git to push updates here and pull from others.

---

## 📄 License

This config is free to use, modify, or fork for personal use.

---

## 🙏 Credits

* [Powerlevel10k](https://github.com/romkatv/powerlevel10k) by @romkatv
* Nerd Fonts by @ryanoasis
* Inspiration from Linux, Kali, and Zsh customization communities
