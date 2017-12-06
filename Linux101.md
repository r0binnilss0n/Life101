 A Beginner Guide To Linux 
===========================
	Hello in this text i will store all usefull information that i find
	while learning & using Linux myselfs, more specificly Debian Stretch so 
	here we go, hope this helps you otherwise it atleas will help me.


 Command lists
-----------------
	Here i will store all commands that i have knowleadge about 
	& will be update as time goes on.

	cd  -> change directory
	ls  -> list directories (also shows file) to show more info add -a
	pwd -> Print name of current working directory
	cp <filePathOne> <filePathTwo> -> copies a file, remember they dont need to have
	the same name, Ex cp fileOne fileTwo will create a file named fileTwo with the
	content of fileOne (fileOne will still excists)
	sudo -> this is something you adds to a command if you get error "premission denied"
	tree -> this command will give a overview of all files and directories structure
	du -sh * -> This will show how much space a file/directory takes on the disk
	du -h 	 -> This command adds all the file/directorys size
	ls | wc -l -> ls you already know, but by adding | wc -l it will now give you a number on how many 	 files there are.
	date -> shows date
        cal  -> shows calendar of current month
        df   -> shows current amount of free space on disk drives
        free -> shows free memory
        file -> Determine file type
        less -> View  file contents
                ¤ Page Up or b - scroll back one page
                ¤ Page Down or space - scroll forward one page
                ¤ Upp Arrow - scroll down one line
                ¤ G - Move to the end of the text file
                ¤ 1G or g - Moves to the beginning of the text file
                ¤ /charachters - search forward to next occurrence of characters
                ¤ n - Search for the next occurrence for the previous search
                ¤ h - Display help screen
                ¤ q - Quit less)
      
        mv   -> Move/rename files and directories
        mkdir-> Create a new directory
        rm   -> remove files and directories (sometimes -d (option) is needed to remove dir)
        ln   -> Create Hard and symbolic links
        type -> Indicates how a command name is interpreted
        which-> Displays which executable program will be executed
        help -> Get help from shell builtins
        man  -> Display a commands manual Page sections is shown below
                ¤ 1 = User commands
                ¤ 2 = Programming interfaces for kerlen system calls
                ¤ 3 = Programming interfaces for the C library
                ¤ 4 = Special files such as device nodes and drivers
                ¤ 5 = File formats
                ¤ 6 = Games and amusements such as screen savers
                ¤ 7 = Miscellabeous
                ¤ 8 = System adminstration commands
        apropos -> Display a list of approproate commands
        info -> Display a commands info entry
                ¤ ? = Display command help
                ¤ PgUp Or Backspace = display previous page
                ¤ PgDn Or space = Display next page
                ¤ n = Next-Display next node
                ¤ p = Previous-Display previous node
                ¤ u = Up-Display the parent node of the currently displayed
                      node, usally a menu
                ¤ Enter = Follow the hyperlink at the cursor location
                ¤ q = Quit
        whatis  -> Display a very brief description of a command
        alias-> Create an alias for a command (not permanent)
        cat  -> Concatenate file
        sort -> Sort lines of text
        uniq -> Report or omit repeated lines
        grep -> Print lines matching a pattern
        wc   -> Print newline, word and byte counts for each file
        head -> Outputs the first part of a file
        tail -> Outputs the last part of a file
        tee  -> Read from standard input and write to standard output and files




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


	# Wavemon #
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

	
	# Tmux # 
	So this is the secound tool i will introduce and its called tmux, and for me this
	tool completely changed the way i worked with my terminal. What it does is that it alowes
	you to split one terminal into multiple resizable terminal-squares that you easily can change
	between so lets begin:
	
	

	Install: 
		sudo apt-get update && sudo apt-get install tmux

	Using it:

	To start using tmux simply type the command:
	
		tmux

	there you go. Now that you have started tmux lets go through some 
	of the shortcuts to add, move and change between the terminals
	
	Prefix is default in linux (Ctrl + b)
	
	Adding a terminal horizontal:
		prefix + "

	So first press (ctrl + b) then (shift + 2)
	
	Adding a terminal verticaly:
		prefix + %

	Change current terminal:
		prefix and arrow keys



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
