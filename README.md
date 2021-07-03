# postinstall_debian11
A bash script to use on a fresh installed debian11 minimal to install and configure some software

### HowTo
First install a debian 11 minimal. Do not select any desktop environment during install (everything unselected there).
https://cdimage.debian.org/cdimage/unofficial/non-free/cd-including-firmware/
Then download and execute this script:

```bash
su -
apt install git -y
exit
cd
mkdir git
cd git
git clone https://github.com/MystixCode/postinstall_debian11.git
cd postinstall_debian11/
chmod a+x postinstall_debian
./postinstall_debian
```

### All Options
 - Update system
 - Install firewall
 - Install KDE-plasma minimal
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
 - Reboot now
