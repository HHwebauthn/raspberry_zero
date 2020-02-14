To use this project you will need the following.

Rasberry pi // any model I have a zero

Linux installed on Raspberry pi 

I used rasbian becasue at the time of making this Kail viersion does not support wifi on the Zero

Install aircrack-ng 

Everything else should alredy be installed

Next you will need to download everything from the github res to your computer

Once you have the device setup and ready to go
you will need to change the path in the createDB.py and create the data base by running the createDB.py file
python3 createDB.py
to the PATH that you want your database
you will also have to change the PATH in db.py

After that is done you can go ahead and run the WIFI_BLUETOOTH.sh bash file
when running the WIFI_BLUETOOTH.sh file use this syntax 
sh WIFI_BLUETOOTH.sh <time>
input the duration of time you what the scan to run 
Ex). sh WIFI_BLUETOOTH.sh 10s  // scan will run for 10 seconds
Ex2). sh WIFI_BLUETOOTH.sh 1m  // scan will run for 1 min
it will run through everything on its own. 
the first time you run the bash file you will be asked to enter a password
this is because it is requiered to start the bluetooth service

you can query the information from the database to verify that everything is being saved correctly
There is a file called readDB.py just run that file and it should report everything thats been saved