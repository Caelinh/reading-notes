# Notes for BASH

## The command line
- The up and down arrows can bring up past entries to use again
- typing echo $SHELL displays current bash version.  

## Basic navigation  
- the command pwd(print working directory) will display the current directory.  
- ls -l will display long listing which will breakdown specific properties about the listed files.  
- / is the very top of the hierarchal structure and known as the root.
- Paths can be relative or absolute.  
**Absolute always begins with a /**  
**relative specifies a location based on the current directory your in.**  
~ (tilde) - This is a shortcut for your home directory. eg, if your home directory is /home/ryan then you could refer to the directory Documents with the path /home/ryan/Documents or ~/Documents  
. (dot) - This is a reference to your current directory. eg in the example above we referred to Documents on line 4 with a relative path. It could also be written as ./Documents (Normally this extra bit is not required but in later sections we will see where it comes in handy).  
.. (dotdot)- This is a reference to the parent directory. You can use this several times in a path to keep going up the hierarchy. eg if you were in the path /home/ryan you could run the command ls ../../ and this would do a listing of the root directory.  
- If cd is run without an argumnent it returns home.
- Hitting tab while typing can initiate autocomplete. If nothing shows that means there are multiple options and tab can cycle between them.  

## More about files  
- Everything that a computer uses is a file. The monitor is a file thats only written to and the keyboard is a file that is only read from.
- linux can read the contents of a file and treat it as such. The name extension doesn't matter.
- Linux is case sensitive
- If naming something with a space, use quotes around it.  
- the \ is an escape character and the space after it won't have the rules followed.  
- if the file name begins with . it will be hidden.

## Manual pages
- typing man<command to look up> displays a manual for that command.
- ````man -k <search term>```` to find a command using key words

## File Manipulation

- the command -p during a mkdir will create the required parent when creating the directory. Also -v  will display exactly what is being created.  

**There are many reasons why we may want to make a duplicate of a file or directory. Often before changing something, we may wish to create a duplicate so that if something goes wrong we can easily revert back to the original. The command we use for this is cp which stands for copy.**  
````cp [options] <source> <destination>````

## [Cheat Sheet](https://ryanstutorials.net/linuxtutorial/cheatsheet.php)  
