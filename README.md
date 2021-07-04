# postinstall_debian11
Script to install debian 11 minimal with selected software and configs

### HowTo

 1. Write debian 11 iso to usb stick:
 - https://www.balena.io/etcher/
 - https://cdimage.debian.org/cdimage/unofficial/non-free/cd-including-firmware/bullseye_di_rc2+nonfree/amd64/iso-cd/
 2. Boot from usb stick and install debian 11 minimal without desktop<br><img src="/img/minimal.png" width="50%" height="50%">
 3. Login as root
 4. Download and start script
```bash
apt install wget -y
su <yourusername>
wget -O postinstall_debian https://raw.githubusercontent.com/MystixCode/postinstall_debian11/main/postinstall_debian
chmod a+x postinstall_debian
./postinstall_debian
```

### All Options
 - update_system
 - install_firmware (amdgpu)
 - install_kde_plasma_minimal
 - reboot_now
 - install_firewall
 - install_steam
 - install_graphic_software (gimp krita blender)
 - install_go
 - install_qemu_kvm
 - create_bridge (network bridge for qemu/kvm)
 - install_more_software (keepass2 thunderbird obs-studio baobab nethogs webext-ublock-origin-firefox ark kcalc kde-spectacle okular gwenview)
 - disable_wifi
 - disable_bluetooth
 - enable_airplane_mode
 - disable_history
 - disable_mouse_acceleration
 - configure_dolphin
 - configure_firefox
 - change_taskbar
 - install_minimal_menu
 - configure_lockscreen (Timeout 10min)
 - change_global_theme_dark
 - change_global_theme_light
 - change_wallpaper
 - restart_ui
