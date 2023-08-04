# Ubuntu-Kylin-23.04
Install OEM mode, encryption and more

20230804 Install Ubuntu Kylin 23.04

- Install OEM “name” – language english
- Select language again English US – keyboard US
- No connection to internet recommended
- Select Normal Installation
- Select Something else

1. Select disk -> New Partition table (fresh install)
2. Select "Free Space" of disk for every partition (case)
    [use + to add and watch for Change button]
(a) 733MB,  Primary,  Use As: EFI System Partition
(b) 2GB, Ext4, /boot (Primary Partition)
(c) ...
	- First, add 115GB as Physical volume for encryption
	- Second, Change the device mapper to Ext4 / (root) 
	The encrypted result is:
	115GB, Ext4, / (root) (Primary Partition)

After reboot, the OEM installation is pending changes to achieve a final custom-touch.

This finalization is important! -- Do not click yet on "Prepare for Shipping" since that is the final process to install the Kylin desktop. Recommending that after adding software it is wise to burn an image of the OEM to save all added goodies that work.

1. Settings → System (case)
(a) Power, adjust as desired usual for laptops “Battery Level” is lower (than): 9%
(b) Display: brightness to 70% works better for human eye
- resolution for laptops should not be as small as a mobile phone or pads.
- zoom may be added for better fit of human eye but we do not have zoom yet.

2. Settings → Personalized (case)
(a) Screensaver, some cases is never the default between pictures or solid color;
(b) Font, 12, 14 due to use of laptop or workstations
(c) add your favorite background picture (a  .jpg format works)
(d) Background, add solid colors of choice or other pictures

3. Settings → Network
Note: Priorities are wired network interfaces thereafter wireless. Since user is plugged in via wired, the system should have provided the user with all sorts of custom settings in the category of wired. Only if user is not plugged in, the system is looking for psychical network interface (PNI) in device-driver for capabilities of wireless. User in general is accustomed to unplugging from wired connection to desired wireless. Unfortunately, such routine is missing in the latest release of Ubuntu Kylin 23.04 and perhaps Ubuntu OS.

As a last user-preference, the right-click on the Task-Bar to select Options eg Adjust Size to medium may serve users. However, Zoom features should take care of many user-options and it is recommended to adjust the desktop per classical incremental standards eg 100% is normal while others need 125%, 150%, 175% even 200%. 

From this point on the system is ready to add software (packages) and internet connection is a must unless such packages are saved on other media or local network.

Since not all packages are delivered by Kylin 23.04, the recourse is Gnome: (via terminal)
apt-get update && apt-get upgrade -y
apt-get install gnome-software -y

Balena Etcher is widely used: (root provided CMDs via terminal)
- get Balena Etcher from github
cd /home/sananton/Downloads/
wget https://github.com/balena-io/etcher/releases/tag/v1.18.12/balena-etcher_1.18.12_amd64.deb
apt install ./balena-etcher_1.18.12_amd64.deb 

- where path is /home, preinstalled by Kylin desktop, followed by user name and the well known Downloads folder.

If the download is executed via browser, just issue the CMD in the terminal
cd … to downloads
apt install ./balena-etcher_1.18.12_amd64.deb 

Now, the Kylin desktop noticed the changes and wants to upgrade. However prior upgrading, look in the UKUI Menu for the Balena Etcher and create a shortcut on desktop eg right-click on the listed item in the  UKUI Menu to create shortcut.

Once done it is time to let Kylin upgrade/update. Reboot.

OEM Kylin install works very good so far even when adding software not in its package application library.

Cases for VLC media player, Printer drivers, Brave Browser and other goodies if apt CMD is not delivering, checkout for packages provided by snap: (although snap is not one of San Anton favorite tool)

Photo shop alternative example:
snap install gimp  # version 2.10.30, or
apt install gimp  # version 2.10.34-1

Good luck,
San Anton 20230804 Canonical? my final word is that Kylin is not an alternative to “MS-winds”, it is actually a better desktop.
PS: download from here there [:0)]
https://cdimage.ubuntu.com/ubuntukylin/releases/23.04/release/
website：https://www.ubuntukylin.com/downloads/download-en.html
MD5(Enhanced):0145d61dcea77cd7e7ced4020e09c840
