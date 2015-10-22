# GitHub Tutorial

_by Evelyn Ariza_

---
## Git vs. GitHub
* **Git**  
is for version control, which is mostly for personal use, so you are able to organize your code. Git is also used on  
the command line and you can use git to take snapshots of your code. 
* **Github**  
is more for collaboration, and you can store your code in the cloud. Github also tracks changes in your code  
and you are able to collaborate with others in the web, if anyone adds changes or deletes any code you are able to  
track the changes made. *Github cannot work without git*.


---
## One-Time Setup
####Creating a Github Account
* Creating a Github account adds snapshots of your code up to the cloud and allows others to look, clone, and modify your code. sign up by entering your  
email address and a password.

####SSH Key 
* the _Secure Shell_ or _Secure Socket Shell_ will generate on your github when you create a new repository, The SSH keys allows you  
to get access to your files on a local machine when you put your files on a remote. To add an SSH Key to your Github you must get the SSH key from your remote machine  
and add it to your github. then to add the key to your remote you put ```ssh -T git@github.com``` to your remote's command line.

####`git config`
* `git config` is important to be setup because it is where git gets your information in order to make a commit. to setup you have to put down:  
```git config --global user.name " First Name Last Name"```   
```git config --global user.email "email address"```


---
## Repository Setup
####Setting up your Repository
1. to initialize git you must be on the command line and type `git init` this allows you to basically start up git in your repository.
2. practice adding and commiting by making a new repository and adding a file called README.md.
3. and any text to your README and save the changes to your file.
4. then add your README to be staged by typing in `add README.md`
5. use git status to make sure your file is staged.
6. once you know your file is staged, commit it by typing `git commit -m "short present tense message on what you did"`  
7. finally type `git push` and you have done your first add & commit!  

####Remote
* A remote is connecting the repository that you are currently in to an external repository, in this case, github.

---
## Workflow & Commands
When you are working on any of your projects you must make sure you are always checking on what is going on in your repository.  

* `git status` allows you see if any of your projects are staged and ready to commit and if it was edited. it is important to use `git status` in order to  
not make any mistakes when commiting your project  
  * **Example**  
```username-repository:~/workspace/github-tutorial (master) $ git status  
On branch master  
nothing to commit, working directory clean```
* `git add` is used to add your current file to be staged. Once your file has been staged, its ready to be committed.  
  * **Example**  
``` git add fil.ext``` or ```git .``` (adds directory that you are currently in.)   

* `git commit -m "message"` this command takes a snapshot of your code after it is stage. Adding a short present tense message is helpful because if you forgot  
 what you committed the day before or someone wants to know what you modified in your code, adding a message allows you and others to know what was done.  
  * **Example**  
```git commit -m "add new directory"```  

* `git push` is used after you have staged, and committed your repository. using push means you are pushing your changes to the cloud and your github, where the  
public is able to see your most recent changes.  
  * **Example**  
```git push``` the command will let you know once your repository has been pushed.