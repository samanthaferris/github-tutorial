# GitHub Tutorial

_by Samantha Ferris_

---
## Git vs. GitHub
 * **Git** is used to create "snapshots" of code. It is used to reload code. Git runs in the command line and you can use it for many things. You can create and organize files, edit them, and eventually commit. This is used to store the code you have created in the cloud. 
 
* **GitHub** is used to store code into the cloud. You can keep track of changes and collaborate on files. 


* **Git** does _**not**_ require GitHub in order to work, _but **GitHub** requires **Git**._

---
## Initial Setup
For the initial setup, you need to connect your c9 account to GitHub. Here are the steps to doing that.
First, you must create a GitHub account. When you're done with that you can create a SSH Key for c9!

* Go to GitHub and click the profile icon at the top right, go to settings and look at the left sidebar. You should see "SSH and GPG keys" section. Click on that.

* When you're done with that, click on "New SSH key", title it "cloud9". 

* Switch to your c9 tab, click the right gear then open "SSH Keys". Copy and paste your SSH key into GitHub. It should start with **ssh-rsa**. Add the SSH key. 

* Finally, open your folder and check by typing "ssh -T git@github.com" you should get the message, "Hi **username**! You've successfully authenticated, but GitHub does not provide shell access." This is fine, that means it worked!



---
## Repository Setup
 To create a repo you must do the following:

*  cd into workspace and make a file called "first-repo".
    * cd ~/workspace
    * mkdir first-repo
    * cd first-repo
    * git init
    
* After that, add a README file.
    * touch README.md
    * open the README 
    * save, add
    * git commit -m "messsage". Make sure it makes sense! That is gonna help you out a lot.
Now, we have to make the remote repo. go to GitHub and find "New repositor" It should be in the top-right. Name it **first-repo**. You names should _always_ match. 
Create your repository.
When you're done. Clck on "SSH". This is a lot better than HTTPS. Copy and paste the two links into your command line.

## Workflow & Commands
 We use a lot of commands in git. Here are some that we use on a daily basis.
 
#### Savng work onto GitHub
Here is the work flow for savng your code onto the site.
    git add file name
    git commit -m "message relevant to what you did"
    git push
This is used constantly so it's something that you should remember.

### Stuck?
    q (while in git log) - Escape

    ctrl x - Leave commit

### Commands
Here are some helpful commands to know. 
    git status - this is a way to see what you've done recently while coding. You can use it to check many things. This is helpful to remember because it does not change your code in anyway.
    
`cd` - Changes directory.
        .. - Goes up one level to the parent directory.
    
`mkdir` - Creates a new directory.
    
`rmdir` - Removes a directory.
    
`touch` - Create a new empty file.
    
`rm` - Removes a file.
    
`rm -rf` - This removes a file with force. Everything in the file will be deleted with no questons asked.
    
`mv` - Rename a drectory.
    
### Git and GitHub Commands
`git init` - Initalize a repostory.
    
`rm -rf .git` - Uninitalize
    
`git add` - Adds a file to the commited stage.
    
`git add --all` - Includes all changes.
    
`git commit` - Record the code.
    
`git push` - Used to push changes to the remote repostory.
    