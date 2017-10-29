 A Beginner Guide To Linux 
===========================
	Hello in this text i will store all usefull information that i find
	while learning & using Linux myselfs, more specificly Debian Stretch so 
	here we go, hope this helps you otherwise it atleas will help me.


 Command lists
-----------------
	Here i will store all commands that i have knowleadge about 
	& will be update as time goes on.
	cd = change directory
	pwd = present woring directory
	cp <filePathOne> <filePathTwo> = copies a file, remember they dont need to have
	the same name, Ex cp fileOne fileTwo will create a file named fileTwo with the
	content of fileOne (fileOne will still excists)
	sudo = this is something you adds to a command if you get error "premission denied"




 Alias
-----------------
	While using linux you will use the linux terminal to almost everything, 
	and you will learn to love it eventually. A step in the right direction
	when using Linux terminal is when you discover Alias'es, an alias is a command
	that executes a predefined command line.

	Ex, i myself uses "upp" to execute 
			'sudo apt-get update && sudo apt-get upgrade'
	this is just one example of how to use it, to set it up start with
	the command: 
	vim ~/.bashrc (vim is the editor i use & highly recommend you do so to)

	Then i usally scrolls to the bottom, and makes a comment to store
	my own alias under lookes something like this.
	 __My Custom alias__
	alias upp='sudo apt-get update && sudo apt-get upgrade'


	then press ESC and type :wq
	For some systems this is when you are done, but sometimes this is not enought
	you might just needs to run the file... yup i mean run it by typing
	. ~/.bashrc

	There you go, now your alias upp or whatever you created should work.





 Tools
---------------
 Here i will store Linux tools im using.


 To start of i will introduce a program called Wavemon, a program that helps
you get a overlook at how your wifi connection is, information like ip, Link 
quality, signal level/strength an much more.
I found this tool while me and my friends tried to find the best spot for our 
router to be placed, and looked at signal levels and link quality to decide.
Lets get to it:


Install:
 -> sudo apt-get update
 -> sudo apt-get install wavemon

and thats it.

Using it.
 -> wavemon (yeah the command is that simple)

There is also some commands when wavemon is running:

Scan window (f3 or 's')
 -> This shows access points and other wireless clients, each entry
 starts with the ESSID, followed by the colour-coded MAC address.
 green/red MAC indicates an (un-)encrypted access point and changes to 
 yellow for non-access points.

Preferences (f7 or 'p')
 -> This allows you to change all program options such as interface and
 level scale parameters. Select a parameter with and , then change the 
 value with and .

Help (f8 or 'h')
 -> This page might show an online-help

About (f9 or 'a')
 -> Release infromation

Quit (f10 or 'q')
 -> Exit wavemon

There you go, now you can keep your network under control like a pro.... kinda






 LINKS 
---------------
	Here i will store links that i used to learn everything i know about Linux
	and i recommend you too takes alook at.

	---> 15 Linux Terminal Commands, cool/good to know <---
	- https://www.lifewire.com/linux-terminal-commands-rock-your-world-2201165 -


	---> Basic Info, Wery good to read, alot of great info <---
	- https://www.lifewire.com/beginners-guide-to-linux-4090233 - 

###########Linux Fedora Asus k501ux####################



###Wifi fix#######
Reference: https://ubuntuforums.org/showthread.php?t=2181558

Code line that fixed my problem: 
 - echo "options asus nb wmi wapf=4" | sudo tee /etc/modprobe.d/asus nb wmi.conf
 
 
 
 
 /*More to come just wait */
