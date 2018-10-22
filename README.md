## GitHub Tutorial

_by Anthony Baez_

---
### Git vs. GitHub
#### Git 
* keeps "snapshots" of your code. ( Instead of making a new file it saves the file ).
* does not require Github.
##### Git Overveiw
* Runs in the command line.
* Basic workflow
  * You have a file ( they are known as a directory ).
    * We initalize git ( this makes your directory into a repository) [repo for short].
  * Edit your file 
  * add your file.
  * commit your file.
 
#### Github
* Stores code in a cloud that can be refered to form any computer.
* Visually tracks changes and logs it so that the user may check to see if undos are nessesary.
* Easily collaborate with other users on files.
* Requires Git
##### Github Overveiw
* [www.Github.com](www.github.com) 

* Runs in the command line
* Basic workflow
  * inital repository
  * OR start from someone elses repository 
    * Fork/Clone/Push/Pull
  * You can use this [website](www.github.com) to check and interact with your repositorys and changes.
  

---
### Initial Setup
1. If you are BRAND NEW to git and git hub start here! If you already have an account and can sign in start at 3
2. Lets Begin! Start by making a Github account by [clicking here](www.https://github.com). 
3. Lets link that account to cloud 9 (click on the octocat logo when signing in) [Click here](c9.io/login).
4. On the top right there should be a setting gear icon click on it and proceed to connected services. Click the green button that says connect.
5. Hit the plus icon to create a new workspace.
* Name the workspace **github-learning**
* Description : Verson Control and collaboration
* Team : click " Dont set a team for this workspace"
* Template "Blank"
6. Create a workspace
7. If you see `.c9` click the gear icon and uncheck show hidden files.

---

Follow the following directions

Lets Setup your SSH key!
* [Click Here](www.github.com) and sign in.
* Click on the profile icon ( top right ).
* Settings 
* SSH and GPG ( left side bar ).
* New SSH key.
* TITLE : cloud9 ( recommended not to use caps ).
* Switch to your cloud9 tab
* gear icon ( top right ).
* SSH key tab 
* copy/paste the 2nd SSH key to github
  * starts with ssh-rsa
  * add SSH key
* Go to cloud9
* Open github-learning ide
* type in `ssh -T git@github.com`
* You should see `Hi <your username>! You've successfully authenticated, but GitHub does not provide shell access._
`
---
### Repository Setup
Lets make our `first-repo`
follow the instructions 
* `cd ~/workspace` ( Always want to cd into workspace so you know where you are )
* `mkdir first-repo` ( Notice how there are no spaces but instead a dash "-")
* `cd first-repo` ( Always remember **cd into a file after you make it** )
* `git init` ( **know where you are before git init** )
GREAT!
We now need a remote to push to 
follow the instructions
* [Click here](github.com)
* click on the top right plus icon and create a new repository
* Repository Name : first-repo
  * THE NAMES ALWAYS NEED TO MATCH!
* Create Repository 
* Scroll down to 

Lets make a README now!
follow the instructions
* `touch README.md`
* open the README
* add `this is my first repo`
* save ( command + s )
* add 
* commit -m "create README"



---
### Workflow & Commands
##### Vocabulary 
1. **git**: a git command
2. **git init** // initializes git in our directory for version control -- **only do this once at the beginning and know where you are.**
3. **git add file.ext** // add the file(s) to the stage to be committed (_note: git add . adds the current/entire directory: all files that have changes_) will not add any deleted or rename files
(note: **git add --all  includes ALL changes, including deleted files**)
4. **git status** // optional **(recommended!)** command to see which files on the stage are ready to committed (_they will be green if ready if not ready then it will be red_).
5. **git commit -m "short/specific message"** // takes a ‘snapshot’ of the files on the stage. The message should be present-tense and short and simple Example: ("Complete first repo")
6. **remote**: we are setting up a connection between our current repository and an external one (that lives on github)
7. **add**: we are adding the remote repo (as opposed to editing or removing an existing one)
8. **origin**: this is our “nickname” for the remote repo.  “origin” is standard.  In the future, you might need multiple remotes.
9. **URL**: the location of the remote repo.  (Could be HTTPS or SSH). Recomended that user uses SSH, since HTTPS requires a constant log in after pushing a file.
10. **pull**: bring any changes from the remote repo down to the local repo
11. **push**: we are sending our commits from our local repo to our remote repo (up to the cloud: Github)
12. **-u**: means “upstream.” This tells git to remember which remote repo & branch to push our changes to when we type git push in the future.



---
### Rolling Back Changes



---
