# postinstall_debian11
Script and files to install debian 11 minimal with firmware and some software and configs

### HowTo


 1. Write debian 11 iso to usb stick:
 - https://www.balena.io/etcher/
 - https://cdimage.debian.org/cdimage/unofficial/non-free/cd-including-firmware/bullseye_di_rc2+nonfree/amd64/iso-cd/
 2. Boot from usb stick and install debian 11 minimal without desktop
   ![](/img/minimal.png)
 3. Login as root
 4. Download and start script
```bash
apt install wget
su <yourusername>
wget -O postinstall_debian https://raw.githubusercontent.com/MystixCode/postinstall_debian11/main/postinstall_debian
chmod a+x postinstall_debian
./postinstall_debian
```

### All Options
 - Update system
 - install firmware (installs amdgpu stuff)
 - Install KDE-plasma minimal
 - Reboot now
 - Install firewall
 - Install steam
 - Install graphic software
 - Install golang
 - Install qemu/kvm
 - Create network bridge for qemu/kvm
 - Install more software
 - Change wallpaper
 - Change global theme
 - Disable mouse acceleration
 - Configure dolphin
 - Disable wifi
 - Disable bluetooth

