# 🖥️ p10k-config

This repository contains my customized [Powerlevel10k](https://github.com/romkatv/powerlevel10k) Zsh theme configuration, designed for a modern terminal experience with features like OS icons, date and time on separate lines, transparency-friendly colors, and a minimalist clean layout.

> ⚡ Optimized for Kali Linux (WSL), but works across all Linux distros.

---

## 📸 Preview

*Coming soon – add a screenshot to show off your prompt!*

---

## 📦 Dependencies

Before using this config, ensure the following are installed:

### 1. Zsh (if not already)

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

### 2. (Optional) Oh My Zsh

**Oh My Zsh is not required** to use Powerlevel10k or this configuration. However, if you prefer a plugin framework, Oh My Zsh offers an easy way to manage themes and plugins.

> ⚠️ If you already have a customized `.zshrc` (with aliases, plugins, or settings), installing Oh My Zsh will **overwrite** it. Make sure to back up your config before installing:

```bash
cp ~/.zshrc ~/.zshrc.backup
```

Install [Oh My Zsh](https://ohmyz.sh/) with:

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

---
### 3. Nerd Fonts

For icons and symbols to render correctly, install a [Nerd Font](https://www.nerdfonts.com/):

#### 1. Hack Nerd Font

```bash
# Example: Hack Nerd Font
wget https://github.com/ryanoasis/nerd-fonts/releases/latest/download/Hack.zip
unzip Hack.zip -d ~/.fonts
fc-cache -fv
```
---
#### 2. MesloLGS NF Font 

```bash
wget https://github.com/ryanoasis/nerd-fonts/releases/latest/download/Meslo.zip
unzip Meslo.zip -d ~/.fonts
fc-cache -fv
```

#### 🛠️ Configure Your Terminal to Use the Font

> Make sure to restart your terminal after installing the font.

##### 🪟 Windows Terminal (WSL/Kali/Ubuntu)

1. Open **Windows Terminal**.
2. Click the dropdown ▾ → **Settings**.
3. Select your shell (e.g., Kali Linux, Ubuntu).
4. Under **Appearance**, set the **Font face** to:

   * `MesloLGS NF`
   * or `Hack Nerd Font`

##### 🐧 GNOME Terminal (Linux Desktop)

1. Open **GNOME Terminal**.
2. Go to **Preferences** → select your profile.
3. Under **Text**, uncheck **Use system font**.
4. Click the font selector and choose:

   * `MesloLGS NF Regular`
   * or `Hack Nerd Font`

##### 💡 Troubleshooting

* Ensure fonts are in `~/.fonts`
* Run `fc-cache -fv`
* Restart the terminal or your system if fonts don't show



---

### 4. Powerlevel10k

#### ✅ With or without Oh My Zsh

Clone the Powerlevel10k theme:

* **If using Oh My Zsh:**

  ```bash
  git clone --depth=1 https://github.com/romkatv/powerlevel10k.git \
    ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
  ```

  Then set this in `~/.zshrc`:

  ```bash
  ZSH_THEME="powerlevel10k/powerlevel10k"
  ```

* **If NOT using Oh My Zsh:**

  ```bash
  git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ~/powerlevel10k
  ```

  Then at the very top of your `~/.zshrc`, add:

  ```bash
  source ~/powerlevel10k/powerlevel10k.zsh-theme
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

Add it manually at the end of the file if it's missing.

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
