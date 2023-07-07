# Hash-generator-w-Bash
I used the text editor vi to create a new file called md5_hash.sh containing my hash generator.
Note, all Bash scripts begin with the shebang(#!), followed by the path to the interpreter which in this case will be the Bash shell with a default path of /bin/bash

Begin writing code by following these steps:

At the terminal window type: 

vi <file name> 

It opens a blank file which you need to switch into editing mode by pressing i — INSERT — keyword will appear at the bottom left of the screen and indicates that you are in insert mode.

Type the shebang and shell interpreter definition #!/bin/bash


Next line type the following:

read -p ”Enter the string to hash: “ input_string
#Generate the MD5 hash
Hash=$(echo -n “$input_string” | md5sum)
Echo “Hash: $hash”


Save the above code into a file name hash_generator.sh.
Make the file executable by running chmod +x hash_generator
It will prompt you to enter the string you want to hash.
Once you enter the string and press Enter, it will display the MD5 hash of the input string.
You can modify this script to use other hashing algorithms like SHA-1, SHA-256, etc., by replacing md5sum with the appropriate command (eg. sha1sum, sha256sum).
