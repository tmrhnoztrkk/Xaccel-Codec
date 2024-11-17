# Xaccel-Codec

Cracked versions of Xaccel-Codec

#Install Xaccel

STEP 1: Upload
Upload file "xaccel-4.3.19.sh" in /home/

https://drive.google.com/drive/folders/19RXgct_-xKyT6XM0sy0Czs14btzlp4rJ?usp=sharing

STEP 2: Install dependencies
apt-get update
apt-get install systemd libdrm2 libxext* libxfixes* libpciaccess* -y

STEP 3: Commdands SSH (In root)
cd /home/
chmod a+x xaccel-4.3.19.sh
bash ./xaccel-codec-4.3.19.sh -i
NOTA: After installation done, reboot server.

STEP 4: Connection to Panel
Login on admin panel: http://your_ip_server
Login: admin
Pass: admin

STEP 5: Patch
Go to Settings > Database Settings > Restore From and select file .73mif32k.gz
NOTA: After restore finished, re-login you on panel.

STEP 6: Finished
Enjoy :)

# Patch Fix

fix ffmpeg and libs files to support kid:key and multiples keys

stop all streams .... and replace binary file in bin and lib files in lib

# Install

STEP 1: Upload Upload file "xaccel-4.3.19.sh" in /home/

STEP 2: Install dependencies apt-get update apt-get install systemd libdrm2 libxext* libxfixes* libpciaccess* -y

STEP 3: Commdands SSH (In root) cd /home/ chmod a+x xaccel-4.3.19.sh bash ./xaccel-codec-4.3.19.sh -i NOTA: After installation done, reboot server.

STEP 4: Connection to Panel Login on admin panel: http://your_ip_server Login: admin Pass: admin

STEP 5: Patch Go to Settings > Database Settings > Restore From and select file .73mif32k.gz NOTA: After restore finished, re-login you on panel.

STEP 6: Finished Enjoy :)

# Installation for Ubuntu and Debian (Official Guide)

1) Install the development tools.
apt-get update
apt-get install systemd build-essential -y
apt-get purge nvidia-* -y
apt-get autoremove -y

2) Disable the Nvidia nouveau open source driver.
echo "blacklist nouveau" > /etc/modprobe.d/nvidia-installer-disable-nouveau.conf
echo "options nouveau modeset=0" >> /etc/modprobe.d/nvidia-installer-disable-nouveau.conf
update-initramfs -u
reboot

3) Install the Nvidia driver.
service lightdm stop
nvidia-uninstall --silent
wget http://us.download.nvidia.com/XFree86/Linux-x86_64/460.67/NVIDIA-Linux-x86_64-460.67.run
bash ./NVIDIA-Linux-x86_64-460.67.run --silent --install-libglvnd
