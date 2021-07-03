# postinstall_debian11
A bash script to use on a fresh installed debian11 minimal to install and configure some software

### HowTo

 1. Take 2 usb sticks
 2. Copy this repo unzipped on usb stick 1
 3. Write debian 11 iso on usb stick 2:
 - https://www.balena.io/etcher/
 - https://cdimage.debian.org/cdimage/unofficial/non-free/cd-including-firmware/bullseye_di_rc2+nonfree/amd64/iso-cd/
 4. Insert both usb sticks
 5. boot from usb stick2 and install debian 11 minimal without desktop
   todo here img
 6. login as root
 7. Find usb device
```bash
blkid -o device
```
 8. And mount it (u may need to replace sda1)
```bash
mkdir /media/usb/
mount /dev/sda2 /media/usb 
cd /media/usb
```
 9. Add permission to execute and start the script
    
```bash
chmod a+x postinstall_debian
```
 10. Then start script as nomral user. not root:
```bash
su yourusername
./media/usb/postinstall_debian
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

