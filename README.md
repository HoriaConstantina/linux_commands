## How to use SSH Keys for GitHub


# First Step

- Create a new Repository in GitHub


# Second Step

- cd into .ssh ( cd ~/.ssh)
- ssh-keygen -t rsa -b 4096 -C yourGithubEmail@domain.com
- copy the contents of the id_rsa.pub file ( cat id_rsa.pub )


# Third Step

- go to your GitHub profile and go to Settings
- go to the SSH keys
- Click **Add SSH key**, enter the contents of the id_rsa.pub file
- Enter GitHub password when prompted




## Git commands to push local repository to the remote repository

- create a new directory ( mkdir name_of_the_folder )
- go inside the new folder ( cd name_of_the_folder )
- create a README file ( nano README.md )
- type your desired content inside the README.md file and save it ( CTRL + X )
- after you saved the file type the following: 
	- git init
	- git add .
	- git commit -m "your message"
	- git branch -M main
	- git remote add origin "remote repo URL"
	- git push -u origin main




## More Linux commands

- display linux processes **top**.
- To become root user **sudo su**.
- To see the history of commands **history**.
- To check the status of a process **systemctl status process_name**.
- To stop a process **systemctl stop process_name**.
- To restart a process **systemctl restart process_name**.
- To make a script you must write **#!/bin/bash** at the start of the file and use a .sh file type.
- To run a file type **sudo bash ./file_name.sh** or just **./file_name.sh**.
- To change a files mode to executable **sudo chmod +x file_name.sh**.
- Once executable, run a script by making it **sudo ./provision.sh**.
- To view a snapshot of the current processes **ps**
- To kill a process **kill [process id]**
- **kill -9** Meaning the process will be killed by the kernel; this signal cannot be ignored. 9 means KILL signal that is not catchable or ignorable
- sudo chmod +x file_name makes the bash file executable
- ll or ls -al to check the permissions of the files
- File permissions: 
	- r - gives read permission 
	- w - gives write permission 
	- x - gives executable permission
	- 777 - gives full control
	- 400 - allows the owner to read
	- 600 - owner can read and write
- Tail is a command which prints the last few number of lines (10 lines by default) of a certain file, then terminates.
- Head command will obviously on the contrary to tail, it will print the first 10 lines of the file.
- The sort command arranges text lines in useful ways. This simple tool can help you quickly sort information from the command line.
- nl - Sometimes you may required to count number of lines in a file on Linux command line or shell scripting.
- wc - The wc command as described can be used to get the number of newlines, words or bytes contained in a file specified.
- The “pipe” command is readily available on UNIX/Linux platforms. This command pipes the output of the previous command to the next command. There are literally TONS of situations where this method offers serious value.Before jumping deeper, there’s something to know of. Every single program in the UNIX/Linux system has 3 built-in data streams.
	- STDIN (0) – Standard input
	- STDOUT (1) – Standard output
	- STDERR (2) – Standard error
	- When we’re going to work with “pipe” tricks, “pipe” will take the STDOUT of a command and pass it to the STDIN of the next command.
- Wildcard Pattern Matching
- ? – matches any single character * – Matches any sequence of characters (including the empty sequence)

### Example (Wildcard)
- Text = "baaabab",
- Pattern = “*****ba*****ab", output : true
- Pattern = "baaa?ab", output : true
- Pattern = "ba*a?", output : true
- Pattern = "a*ab", output : false 
- Reference

- How to Hide Files
- The period (.) at the beginning of the new filename indicates that it’s hidden:

- mv test.txt .test.txt
- To verify the file is now hidden, display the contents of the current directory:

- ls –a
