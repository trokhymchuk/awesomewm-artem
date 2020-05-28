# AwesomeWM- artem
Fork of material-awesome (https://github.com/ChrisTitusTech/material-awesome).

## To install (Arch? Arch-based):
### Packages
- AwesomeWM as the window manager - `awesome`
- Roboto as the font - `ttf-roboto`
- Rofi for the app launcher - `rofi`
- Compton for the compositor (blur and animations) - `compton`
- i3lock the lockscreen application - `i3lock`
- xclip for copying screenshots to clipboard package - `xclip`
- gnome-keyring - `gnome-keyring`
- polkit - `polkit`
- pulseaduio for sound control - `pulseaudio`
- brightnessctl for brightness control - `brightnessctl`
- Materia as GTK theme - `materia-theme`
- Papirus Dark as icon theme Universal Install - `wget -qO- https://git.io/papirus-icon-theme-install | sh`
- lxappearance to set up the gtk and icon theme - `lxappearance`
- kde-spectacle - `spectacle`
### Configuration
Clone from repository - `git clone https://gitlab.com/artemtrokhymchuk/awesomewm-artem.git ~/.config/awesome`

## Audio control
1. Install pulseaudio
2. Run `pactl list sinks short` and chek yor output (default is 0)
3. Then change default output in the  configuration/keys/global.lua in the 283 and 291 lines
4. Then change default output in the  widget/volume/volume-slider.lua in the 18 line

## Backlight control
1. Check your GPU model - `ls /sys/class/backlight/`
2. Change default (amdgpu_bl1) in the configuration/keys/global.lua in the 266 and 274 lines
