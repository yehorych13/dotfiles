# Hyprland dotfiles

Welcome to my Hyprland + Arch Linux dotfiles repository! This setup is designed for a minimal [Arch Linux](https://wiki.archlinux.org/title/Arch_Linux) install.

## Installation

**Warning:** Before proceeding, please be aware that using these dotfiles may result in an unstable or non-functional system.  Ensure you have a backup of your current configuration and important data before running any scripts.

1. Copy repository
```shell
git clone https://github.com/yehorych13/dotfiles && cd dotfiles
```
2. Install all packages from `pkgs.txt` I recommend using [yay](https://github.com/Jguer/yay) for this. (One day I will make an automatic script for this, but for now, do it manually)
 
3. Use the installation script to move your current configuration to a backup folder located in `~/.config/backup_{date}` and create symlinks for these dotfiles.
```shell
chmod +x install.sh && ./install.sh
```

4. Set zsh as the default shell
```
chsh -s $(which zsh)
```

5. Enable SDDM reboot you system and that's it!
```shell
sudo systemctl enable sddm
sudo reboot
```

## Keybindings
|Description|Keybinding|Alternative Keybinding                        
|----------------|-------------------------------|-------------|
|Main mod        |`SUPER`                        ||
|Open terminal   |`SUPER + ENTER`            ||
|Open file manager|`SUPER + E`||
|Open app menu|`SUPER + R`||
|Open theme selector|`SUPER + ALT + T`||
|Take a screenshot|`SUPER + SHIFT + S`||
|Kill active process|`SUPER + Q`||
|Kill active process anyway|`SUPER + SHIFT + Q`||
|Exit from hyprland|`SUPER + SHIFT + DELETE`||
|Toggle floating mode|`SUPER + T`||
|Toggle fullscreen mode|`SUPER + F`||
|Pseudo|`SUPER + P`||
|Toggle split|`SUPER + J`||
|Resize window|`SUPER + SHIFT + up/down/left/right`||
|Move window|`SUPER + LMB`|`Mouse 5`|
|Resize window|`SUPER + RMB`|`Mouse 4`|
|Move focus|`SUPER + up/down/left/right`|
|Switch between workspaces|`SUPER + 1..0`|
|Move active window to workspace|`SUPER + 1..0`|
|Scratchpad(special workspace)|`SUPER + S`|
