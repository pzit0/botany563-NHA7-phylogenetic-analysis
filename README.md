# botany563-NHA7-phylogenetic-analysis
Folder dedicated to the class Botany564 on spring 2023. I will be analyzing the NHA family in e. affinis and other species

# CLASS NOTES: GITHUB 101

## PERSONAL TOKEN: 
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

## Jan 27, 2023: Learning how to use github 
Create a new repository on the github through the default nagivator 
Then copy the url and input the following code on the terminal 

$ git clone Desktop/https://github.com/pzit0/botany563-NHA7-phylogenetic-analysis.git 

So far this has created a usable repository on both github server and my local computer 
By writing this here, I am changing the README.md file on my local computer 
I am guessing that I will then learn how to update the version on the server

Yes, these are the three secret commands: 
$ git add README.md
$ git commit -m "updated readme" 
$ git push

## Jan 31, 2023: Learning how to fork, clone, pull and fetch 
When you want to use and modify someone else's repository you first need to fork and clone it
To fork it you can go to the repository on your default navigator 
click on fork (nothing will happen) 
Then go to your terminal and go to your folder of choice
you can then clone it using the following command: 

$ git clone https://github.com/pzit0/phylo-class-social dummy

the first argument is what you'd like to clone and the second one is how you want the folder to be called
pay attention. make sure you're cloning your OWN forked repository, not the original one/ upstream 

you can confirm if this happened by using the following command inside dummy/: 

$ git remote -v

Expected output: 

origin	https://github.com/pzit0/phylo-class-social.git (fetch)
origin	https://github.com/pzit0/phylo-class-social.git (push)

Notice that the owner is pzit0, NOT crl4.

Now you have to sync it up to the original repository. You can do this by using the following command: 

$ git remote add upstream https://github.com/crsl4/phylo-class-social

if you'd like to update your cloned repository according to the changes made on the original repository, use the following command: 

$ git pull upstream master 

This changes your files!! if you'd rather not change your files (download and keep yours), use: 

$ git fetch upstream master 

if you'd like the original repository to pull YOUR changes, you can pull request on github online
You must first do git add/ git commit/ git push 
This will update your remote repository with your local changes
Then you can git pull request on YOUR page (online) to upstream

