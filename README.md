# postinstall_debian11
Script to install debian 11 minimal with selected software and configs

### HowTo

 1. Download Debian 11
 - https://cdimage.debian.org/cdimage/unofficial/non-free/cd-including-firmware/11.1.0+nonfree/multi-arch/iso-cd/firmware-11.1.0-amd64-i386-netinst.iso
 2. Write debian 11 iso to usb stick using either Balena Etcher or the DD command (replace /dev/sda with your usb device!):
 - https://www.balena.io/etcher/
```shell
lsblk -f
sudo dd bs=4M if=$HOME/Downloads/firmware-11.1.0-amd64-i386-netinst.iso of=/dev/sda oflag=sync status=progress
```
 3. Boot from usb stick (use a usb2 port usb3 doesnt seem to work) and install debian 11 minimal without desktop<br><img src="/img/minimal.png" width="50%" height="50%">
 4. Login as root
 5. Install git
 ```bash
apt install git
su <yourusername>
git config --global user.name "Sarah Smith"
git config --global user.email "sarah.smith@email.com"
cd
mkdir Git
cd Git
 ```
 6. Download this repo and start script
```bash
git clone https://github.com/MystixCode/postinstall_debian11.git
cd postinstall_debian11
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
 - install_firefox (firefox-esr webext-ublock-origin-firefox)
 - install_more_software (keepass2 thunderbird obs-studio baobab nethogs ark kcalc kde-spectacle okular gwenview)
 - remove_software (kwalletmanager termit xterm kdeconnect)
 - disable_wifi
 - disable_bluetooth
 - enable_airplane_mode
 - disable_history
 - disable_mouse_acceleration
 - configure_dolphin
 - configure_firefox
 - install_minimal_menu
 - configure_lockscreen (Timeout 10min)
 - change_global_theme_dark
 - change_global_theme_light
 - change_wallpaper
 - restart_ui
