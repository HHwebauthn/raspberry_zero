This collection of files is used for scanning nearby WIFI and Bluetooth devices and saving the unique identifiers to a sqlite3 database.


First setup the database file by runing creatingDB.py, remeber to change the Path you want your database to be. 
You must also change the Path in the DB.py file to the same Path you set for creatingDB.py

in the terminal you will need to type
'service bluetooth start'
I put this command in my bash file but it requieres a pass word on raspbian to start.



next run the bash file named WIFI_BLUETOOTH.sh
you can change the bash file as you need.


after runng the bash file everything should be saved to the database.


Things to install on raspberry pi.

I used rasbian as my OS.

sudo apt-get install python3
sudo apt-get install python3 sqlite3
sudo apt-get install network-manager
sudo apt-get install network-manager-gnome


I had to reboot my raspberry pi to get network manager to display information using 'nmcli d wifi' 

my .py file requieres network manager to be installed and working correctly and it need to have 'service bluetooth start' on so the bash file can run 'hcitool -i hci0 scan'
to scan for blue tooth devices.


change things as you wish.


