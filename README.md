
# Recommnded Apps



# Recommended Utilities

neofetch

      sudo apt install newfetch

      neofetch

imager    

      sudo apt install rpi-imager

gparted

      sudo apt install gparted

Botspot PiApps link on GitHub 

      https://github.com/Botspot/pi-apps
      
      git clone https://github.com/Botspot/pi-apps

      ~/pi-apps/install


# Other

pikiss

block 60fps videos in chromium

NTFS support:   ntfs-3g

Resource monitor alternative:  gnome-system-monitor

System info GUI:  hardinfo (lshw-gtk, sysinfo)

System info CLI:  inxi (inxi -Fx), lshw, hwinfo


      

.

# Helpful commands

Hardware and OS:   uname -a

hardware: uname -m   (shows if you are running 64 bit)

hardware: gpio -v

CPU: uname -p

OS: uname -o

computer name: hostname

serial number: cat /proc/cpuinfo | grep Serial

OS: cat /etc/os-release | grep PRETTY | cut -d'"' -f2


# Networking:

IP address: hostname -I

LAN IP : ifconfig eth0 | grep "inet "

WAN IP: ifconfig wlan0 | grep "inet "

list wifi AP:  sudo iwlist wlan0 scan | grep ESSID | cut -d: -f2 | sort | uniq

# Update software:

        sudo apt update

        sudo apt upgrade

        sudo apt autoremove

        sudo apt full-upgrade

        sudo rpi-update  (only if needed)


Raspberry pi 400 firmware update

      sudo apt update

      sudo apt dist-upgrade

      sudo apt install rpi-eeprom

      sudo rpi-eeprom-update




# Printing

Printer support:  cups and system-config-printer

HP drivers including P1606DN and C3600 basic:  hplip

HP Color 3600 driver: printer-driver-pxljr

Brother printer – https://support.brother.com/g/b/downloadlist.aspx?c=us&lang=en&prod=lpql810weus&os=130

DYMO: printer-driver-dymo

Zebra:


