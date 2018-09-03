* #### root, home
    * `/`  -> root directory
    * `~`  -> "home/{user_name}/" directory, where user_name = name of the user say abhi.
* copy and move a file
	- copy using `cp source/location destination/location`
	- move using `mv source/location destination/location`
	
	<br/>
#### NOTE: Although a file can be copied or moved into the Ubuntu folder in C:\ drive. But, one should not do that because it will not show in the folder in ubuntu file directories, when accessed via `bash-cmd`.
		
* #### `uname -a`
	**o/p** - displays the system architecture. Here, x86_64 means the system is 64-bit. If you will get i386 or i686 then the system is 32-bit. 

	Linux Abhijit 4.4.0-17134-Microsoft #137-Microsoft Thu Jun 14 18:46:00 PST 2018 x86_64 x86_64 x86_64 GNU/Linux

* #### Editor - Install Sublime Text 3 in Ubuntu
	**Method-1: Only linux involved**
    * `cd ~`
    * `wget http://c758482.r82.cf2.rackcdn.com/sublime-text_build-3083_amd64.deb`
    * if 'Unable to load libgdk-x11-2.0.so' , then `sudo apt-get install libgtk2.0-0`
    * Now, `subl` command wouldn't work until added onto the path.
    * the directory in which the sublime text gets installed - "/opt/sublime_text"
	* `ln -s "/opt/sublime_text" /usr/local/bin/subl` [PERMANENT] <br/>
					OR <br/>
	  `alias subl='"/opt/sublime_text"'`	 [TEMPORARY]  Temporary i.e. will exist within that bash window 
	
    **Method-2: Access the sublime (installed in windows) [RECOMMENDED]** 
	* `ln -s "/mnt/f/Softwares/Sublime Text 3/subl.exe" /usr/local/bin/subl` [PERMANENT] <br/>
						OR <br/>
	  `alias subl='"/mnt/f/Softwares/Sublime Text 3/subl.exe"'` [TEMPORARY]- fetching installed repo in windows from ubuntu through WSL due to the [Interoperability](https://blogs.msdn.microsoft.com/wsl/2016/10/19/windows-and-ubuntu-interoperability/) 
      
    
    [SOURCE](http://docs.sublimetext.info/en/latest/getting_started/install.html)
* #### Seach Files, Folders
	```
	find Search-Directory-Path -name file-name-to-search
	
	## only search for files ##
	find Search-Directory-Path -type f -name file-name-to-search
	
	## only search for directories/folders ##
	find Search-Directory-Path -type d -name dir-name-to-search
	```
	E.g.- 
	* `$ find /home/user/ -name xyz`
	* `$ sudo find / -name passwd`
	* `$ sudo find / -type f -name "birthday-party.mp4"`
	* `$ sudo find / -type f -name "*.mp4"`
	* `$ sudo find / -type f -iname "*.mp4"`
	* `$locate resume.pdf`
	
  [Source](https://www.cyberciti.biz/faq/linux-how-can-i-find-a-file-on-my-system/)
	
* #### PATH check
    * `echo $PATH` - with WSL, shows Ubuntu + windows environment variables.
    
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
  
