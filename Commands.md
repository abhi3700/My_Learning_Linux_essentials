* #### `uname -a`
**o/p** - displays the system architecture. Here, x86_64 means the system is 64-bit. If you will get i386 or i686 then the system is 32-bit. 

Linux Abhijit 4.4.0-17134-Microsoft #137-Microsoft Thu Jun 14 18:46:00 PST 2018 x86_64 x86_64 x86_64 GNU/Linux

* #### Editor - Install Sublime Text 3
    * `cd ~`
    * `wget http://c758482.r82.cf2.rackcdn.com/sublime-text_build-3083_amd64.deb`
    * if 'Unable to load libgdk-x11-2.0.so' , then `sudo apt-get install libgtk2.0-0`
    
    [SOURCE](http://docs.sublimetext.info/en/latest/getting_started/install.html)
* #### ```tree -L 1``` 

![](https://github.com/abhi3700/My_Learning_Linux_essentials/blob/master/Images/1.png)

* #### ```tree -L 2```

![](https://github.com/abhi3700/My_Learning_Linux_essentials/blob/master/Images/2.png)

* #### ```CTRL + L``` - clears the screen
* #### ```CTRL + D``` - logout 
* #### ```CTRL + Y``` - Paste
* #### ```sudo apt-get update``` - Update the packages
* #### ```cd /``` - Go to the root 
* #### ```history -c``` - clears the screen, 
  ```history``` - displays the history commands
* #### ```echo``` - prints the word 'hello' after 'echo'.
* #### ```hostname``` - prints the computer name
* #### ```date``` - prints the date
* #### ```bash -V``` - prints the bash's version
* #### ```cd ~``` - takes to the home directory
* #### Opening the explorer within the bash shell like in windows cmd.
	```alias start='cmd.exe /c start'```
   DONE!!.
	Now, open it through - 
	```start .```	

   Note: it will not start an explorer on linux only files, but any mapped windows file systems will work.
   **Source** - https://stackoverflow.com/questions/44245721/launching-explorer-from-wsl

* #### ```sudo nano [Filename]``` - Opens any type of file
  E.g. - ```sudo nano config.ini```
  
