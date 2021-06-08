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

