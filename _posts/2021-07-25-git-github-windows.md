---
layout: post
title:  "Git bash on Windows 10"
author: paul
categories: [ git, tutorial ]
image: assets/images/git-bash-windows.png
---

Commiting codes directly from the local disc to the github repository is an important productivity asset. Let's learn some codes regarding commiting codes through gitbash on Windows 10.

# Git-bash on windows

- download git (commandline interface ) for windows from this site
- [https://git-scm.com/download/win](https://git-scm.com/download/win)
- there will be an unix like terminal installed "gitbash"
- open gitbash
- setup your working directory to the c/git

like: 

```bash
shamr@DESKTOP-SL6NFAN MiNGW64/c/git
```

- login your github account
- create new repository
- name it "testgit" (whatever in your mind)

```bash
$ git config --global [user.name](http://user.name/) "paulshamrat"
$ git config --global user.email [bt20f002@smail.iitm.ac.in](mailto:bt20f002@smail.iitm.ac.in)
```

- [this will ask your credentials and login via browser in which you previously logged into your github account]

```bash
$ git clone [https://github.com/paulshamrat/testgit.git](https://github.com/paulshamrat/testgit.git)
$ ls
$ cd testgit
$ git status
$ git add test.txt
$ git status
$ git commit -m "first commit" test.txt
$ git push -u origin main
```

## Add, commit and push multiple files

```bash
$ git status
$ git add --all
$ git status
$ git commit -m "added 4 new posts" --all
$ git status
$ git push -u origin master
```

# Another note:
- you have cloned repository on your local machine.
- but you have commited from the browser directly.
- then you made changes in your local machine and tried to push the command
- then it wil show, "rejected" sign! so what to do?

```bash
$ git pull --all
```
- So, this command will pull down all changes made in the repository and merged with your local machine and pop-up a message to close the command tab of VS code.
- close the current tab and it pulled down succesfully.
- Now time to push your local changes to your desired repository.

Last update: Jan 19, 2022.

Reference: [https://www.youtube.com/watch?v=J_Clau1bYco](https://www.youtube.com/watch?v=J_Clau1bYco)