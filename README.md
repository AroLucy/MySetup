# MySetup

This is a guide on how to get a Setup like mine

## Screenshot
#### Light 
![](https://github.com/LucyUwI/MySetup/blob/main/66em8kur2rl71.png?raw=true)
####Nord
![](https://github.com/LucyUwI/MySetup/blob/main/a.png?raw=true)
# How to install
[Arch and Arch-Based Distros Setup](#arch) \
[Ubuntu, KDE Neon and other Ubuntu/Debain-based distros Setup](#deb)


[Configuration](#config)

# <a name="arch"></a> Arch

[Installing KDE](#kde-arch) \
[Istalling yay (Optional)](#yay) \
[Installing latte-dock-git (yay)](#ld-yay) \
[Installing latte-dock-git](#ld-arch)

### <a name="kde-arch"></a> Installing KDE

Minimal:
```bash
sudo pacman -S plasma-dektop
```
With aplications
```bash
sudo pacman -S plasma kde-applications 
```
(Optional) Wayland Session 
```bash
sudo pacman -S plasma-wayland-session
```


### <a name="yay"></a> Installing YAY (optional)

1. Install Git
```bash
sudo pacman -S git
```

2. Clone the YAY repository
```bash
$ git clone https://aur.archlinux.org/yay.git
```

3. Build and install YAY
```bash
cd yay
makepkg -si
```

### <a name="ld-yay"></a> Installing Latte-dock-git W/ YAY
```bash
yay -S latte-dock-git
```

### <a name="ld-arch"></a> Installing Latte-dock-git W/O YAY
```bash
sudo pacman -Syu make extra-cmake-modules python plasma-framework plasma-desktop
git clone https://aur.archlinux.org/latte-dock-git
cd latte-dock-git
makepkg -si
```

# <a name="deb"></a> Ubuntu, KDE Neon and other Ubuntu/Debain-based distros

[Installing KDE](#kde-deb) \
[Installing latte-dock-git](#ld-deb) 


### <a name="kde-deb"></a> Installing KDE

Minimal:
```bash
sudo apt install plasma-dektop
```
Full:
```bash
sudo apt install plasma-full
```
Standard:
```bash
sudo apt install plasma-standard
```

(Optional) Wayland Session 
```bash
sudo apt install plasma-workspace-wayland
```

### <a name="ld-deb"></a> Installing Latte-dock-git

#### Non-KDE Neon distros
```bash 
sudo add-apt-repository ppa:kubuntu-ppa/backports
sudo apt update
sudo apt dist-upgrade
```

```bash
sudo apt install git cmake extra-cmake-modules qtdeclarative5-dev libqt5x11extras5-dev libkf5iconthemes-dev libkf5plasma-dev libkf5windowsystem-dev libkf5declarative-dev libkf5xmlgui-dev libkf5activities-dev build-essential libxcb-util-dev libkf5wayland-dev git gettext libkf5archive-dev libkf5notifications-dev libxcb-util0-dev libsm-dev libkf5crash-dev libkf5newstuff-dev libxcb-shape0-dev libxcb-randr0-dev libx11-dev libx11-xcb-dev kirigami2-dev
git clone https://github.com/kde/latte-dock
cd latte-dock
sh install.sh
```

# <a name="config"></a> Configuration


