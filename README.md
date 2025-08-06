# hyprland
# Step 1
```
sudo pacman -S wofi kitty freetype2 zsh git hyprlock swww waybar ttf-font-awesome otf-font-awesome ttf-jetbrains-mono obsidian pavucontrol feh meson nwg-look papirus-icon-theme fastfetch file powerline-fonts inetutils ttf-font-awesome otf-font-awesome ttf-jetbrains-mono neovim code ttf-dejavu bluez bluez-utils blueman telegram-desktop vlc fastfetch

git clone https://aur.archlinux.org/yay.git
cd yay
makepkg -si

yay -S hyprshot wlogout
```


# Step 2
```
cd Докуметы
git clone https://github.com/maters66/hyprland.git
git clone https://github.com/vinceliuice/Graphite-gtk-theme.git
yay -S Rose-Pine
```


# Step 3
```
cd hypr
cp -r kitty waybar wlogout hypr wofi swaylock rofi kitty fastfetch ./config
```


# Step 4
```
cd Документы/Graphite-gtk-theme
./install.sh
```

# Step 5
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git "${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k"
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting


nvim ~/.zshrc
ZSH_THEME="powerlevel10k/powerlevel10k"
plugins=(git zsh-autosuggestions zsh-syntax-highlighting)
source ~/.zshrc

chsh
/bin/zshrc

reboot
```

