<div align="justify">

<div align="center">

```ocaml
 ❄️ hyprland / aurora / catppuccin ❄️
```

tell me if anything's broken lol
# gallery
![image](https://github.com/user-attachments/assets/c7980d56-847f-487f-a3bb-9b053f0f23fc)
![image](https://github.com/user-attachments/assets/e7da2f75-af16-4e95-ab1b-313e679a0f8c)
![image](https://github.com/user-attachments/assets/e6089643-f65a-4a31-a3ca-0ed2f9a6c842)

 

https://user-images.githubusercontent.com/77581181/204240865-8a272152-7c31-45f9-a46b-47099b071060.mp4

 
</div>
</div>




<div align="justify">

<div align="center">

# installation
 
<hr>
 
</div>
</div>

## Arch
dependencies
```
hyprland-git waybar-hyprland-git cava waybar-mpris-git python rustup kitty fish wofi xdg-desktop-portal-hyprland-git tty-clock-git swaylockd grim slurp pokemon-colorscripts-git starship jq dunst wl-clipboard swaylock-effects-git swww-git
```
using `paru`
```
paru -S hyprland-git waybar-hyprland-git cava waybar-mpris-git python rustup kitty fish wofi xdg-desktop-portal-hyprland-git tty-clock-git swaylockd grim slurp pokemon-colorscripts-git starship jq dunst wl-clipboard swaylock-effects-git swww-git
```

## moving config files

```bash
git clone -b aurora https://github.com/starsprinter92/dotfiles-flicko-aurora-fix
cd dotfiles-flicko-aurora-fix
cp -r ./config/* ~/.config
```

## additional setup

```bash
mkdir ~/.config/hypr/store
touch ~/.config/hypr/store/dynamic_out.txt
touch ~/.config/hypr/store/prev.txt
touch ~/.config/hypr/store/latest_notif
cp -r ~/dotfiles-flicko-aurora-fix/local/* ~/.local/

chmod +x ~/.config/hypr/scripts/tools/*
chmod +x ~/.config/hypr/scripts/*
chmod +x ~/.config/hypr/*
```

## building the tools used in this rice

`rgb-borders` | rgb borders for grouped windows
```bash
git clone https://github.com/flick0/rgb-rs
cd rgb-rs
cargo build --release
cp ./target/release/rgb ~/.config/hypr/scripts/
```



