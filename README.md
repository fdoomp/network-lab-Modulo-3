# network-lab-Modulo-3
SOlll Modulo 3

MODULO III PRACTICA 1

sudo nano /etc/default/grub

GRUB_DEFAULT=0
GRUB_TIMEOUT_STYLE=menu
GRUB_TIMEOUT=20

sudo update-grub

sudo reboot

RECOVERY MODE

mount -0 remount, rw /

passwd root

/dev/sda2/ 
 
mount -n -o remount, rw /

fsck -y /dev/sda2 

---------------------------------------------------------------------------------
---------------------------------------------------------------------------------
MODULO III PRACTICA 2


cd /

mkdir Backups2 

cd Backups2 

nano backuplm.sh 

#!/bin/bash

# Obtener la fecha y hora
DATE=$(date +"%d-%m-%Y:%H:%M")

# Crear el backup on tar
tar -czvf "/Backups2/" "$Date".tar.gz" /home/fernando

chmod 744 backuplm.sh 

./backuplm.sh 

tar -xzvf /Backups2/14-10-2025:11:18.tar.gz -C /Backups2/ 

ls

cd home

cd fernando

ls -a

cd Desktop

nano backuplm2.sh

#!/bin/bash 

echo"Cual nombre desea ponerle al archivo" 

read nombre 

ifconfig > /home/fernando/Desktop/$nombre.txt 

chmod 744 backuplm2.sh

./backuplm2.sh

reboot

cd Desktop

cat ModuloIII.txt

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------

