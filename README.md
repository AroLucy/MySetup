# MySetup

This is a guide on how to get a Setup like mine

## Screenshot

![](https://github.com/LucyUwI/MySetup/blob/main/66em8kur2rl71.png?raw=true)

# How to install
[Arch and Arch-Based Distros](#arch) \
[Ubuntu, KDE Neon and other Ubuntu/Debain-based distros](#deb)

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
sudo pacman -Syu
make extra-cmake-modules python plasma-framework plasma-desktop
git clone https://aur.archlinux.org/latte-dock-git
cd latte-dock-git
makepkg -si
```


