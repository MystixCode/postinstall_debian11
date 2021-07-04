# postinstall_debian11
Script to install debian 11 minimal with selected software and configs

### HowTo

 1. Write debian 11 iso to usb stick:
 - https://www.balena.io/etcher/
 - https://cdimage.debian.org/cdimage/unofficial/non-free/cd-including-firmware/bullseye_di_rc2+nonfree/amd64/iso-cd/
 2. Boot from usb stick and install debian 11 minimal without desktop
   ![](/img/minimal.png)
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

 - Update system
 - Install amdgpu firmware
 - Install KDE-plasma minimal
 - Reboot now to start new installed kde / firmware
 - Install firewall
 - Install steam
 - Install graphic software (gimp krita blender)
 - Install golang
 - Install qemu/kvm
 - Create network bridge for qemu/kvm
 - Install more software (keepass2 thunderbird obs-studio baobab nethogs webext-ublock-origin-firefox ark kcalc kde-spectacle okular)
 - Disable wifi
 - Disable bluetooth 
 - Enable airplane mode
 - Disable History
 - Disable mouse acceleration
 - Configure dolphin
 - Change taskbar location to left
 - Install minimalmenu
 - Change wallpaper
 - Change global theme
 - Install sddm theme
 - Configure Screenlock

