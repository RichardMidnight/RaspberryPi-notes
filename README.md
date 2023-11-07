
# Recommended Apps Management Tools

You can put already-installed apps on the menu:
      
      go to "Preferences"  / "Main Menu Editor"
      
 You can install Raspberry Pi recommended apps:
      
      go to "Preferences" / "Recommended Software"  
      
 You can install other Debian software with "Preferences" / "add/remove software" but it can be complicated.
 
 You can install "Botspot PiApps" - Raspberry Pi App Store for Open Source Projects

      https://github.com/Botspot/pi-apps
      
      git clone https://github.com/Botspot/pi-apps

      ~/pi-apps/install
 


# Recommended Apps

TBD


# Recommended Utilities

pisafe - create and flash sd images with a GUI

      wget https://raw.githubusercontent.com/RichardMidnight/pi-safe/main/pisafe
      bash pisafe
      
      Then you can select 'install' from the pisafe menu to install it into the Raspbian menu


"sd" - create and flash sd images

      www.github.com/RichardMidnight/sd


neofetch - show system info

      sudo apt install newfetch

      neofetch

rpi-imager - write image files to sd card    

      sudo apt install rpi-imager

gparted - partition disks

      sudo apt install gparted

catfish - file search

      sudo apt install catfish




# Other

great reference:  https://www.ubuntupit.com/useful-raspberry-pi-commands/

pikiss

CommanderPi

block 60fps videos in chromium

NTFS support:   ntfs-3g

Resource monitor alternative:  gnome-system-monitor

System info GUI:  hardinfo (lshw-gtk, sysinfo)

System info CLI:  inxi (inxi -Fx),  lshw,  hwinfo

Stacer



# Desktop environments

## Install standard Linux Desktop Environments.  watch out - unstable! seems to break wifi and other things
             
Install other desktop environments: 

      sudo tasksel
      
Switch to a different desktop environment:
      
      sudo update-alternatives --config x-session-manager

For a Windows-like experience:

      Install the "KDE/Plasma DE"
      For even more: you can install a windows theme with "global theme"
      
 ## Other options     
       
BotSpot Windows 10 theme - Easy light-weight windows theme
      
      https://github.com/Botspot/Windows-10
      
Twister OS offers great customization to Raspberry pi OS. But not small images

      www.twisteros.com
   
.   

# Helpful commands

Switch to root: sudo su

Add user to sudo group:   sudo adduser <user> sudo

Hardware and OS:   uname -a

hardware: uname -m   (shows if you are running 64 bit)

hardware: gpio -v

CPU: uname -p

OS: uname -o

computer name: hostname

serial number: cat /proc/cpuinfo | grep Serial

OS: cat /etc/os-release | grep PRETTY | cut -d'"' -f2


# Networking:

IP address: hostname -i

LAN IP : ifconfig eth0 | grep "inet "

WAN IP: ifconfig wlan0 | grep "inet "

list wifi AP (may need sudo):  iwlist wlan0 scan | grep ESSID | grep -v '""' | cut -d: -f2 | sort | uniq

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




# Printing (2019)

Printer support:  cups and system-config-printer

HP drivers including P1606DN and C3600 basic:  hplip

HP Color 3600 driver: printer-driver-pxljr

Brother printer – https://support.brother.com/g/b/downloadlist.aspx?c=us&lang=en&prod=lpql810weus&os=130

DYMO: printer-driver-dymo

Zebra:



# Raspberry Pi OS 64 bit  (in beta as of Jan 2021)

Get the 64bit image

      https://downloads.raspberrypi.org/raspios_arm64/images/
      
How do I know if I am running 64-bit Kernel?

      Use neofetch
      
      or
      
      uname -m
      
How do I know if a program is 64-bit?

      which [filename]
      
      file [filename]
      
      example, determine which version of zip you are running
      
      which bash
      
      file \usr\bin\bash
      


