## GitHub Tutorial

_by Anthony Baez_

---
### Git vs. GitHub

Git is a revision system, a tool to manage your code history. GitHub is a workspace for Git repositories. They are not the same thing but Git is the tool, GitHub is the workspace for projects that use Git.

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
1. [Click Here](www.github.com) and sign in.
2. Click on the profile icon ( top right ).
3. Settings 
4. SSH and GPG ( left side bar ).
5. New SSH key.
6. TITLE : cloud9 ( recommended not to use caps ).
7. Switch to your cloud9 tab
8. gear icon ( top right ).
9. SSH key tab 
10. copy/paste the 2nd SSH key to github
  * starts with ssh-rsa
  * add SSH key
11. Go to cloud9
12. Open github-learning ide
13. type in `ssh -T git@github.com`
 You should see `Hi <your username>! You've successfully authenticated, but GitHub does not provide shell access._
---
### Repository Setup
Lets make our `first-repo`


**Follow the instructions**
1. `cd ~/workspace` ( Always want to cd into workspace so you know where you are )
2. `mkdir first-repo` ( Notice how there are no spaces but instead a dash "-")
3. `cd first-repo` ( Always remember **cd into a file after you make it** )
4. `git init` ( **know where you are before git init** )

GREAT!
We now need a remote to push to 
**Follow the instructions**
=======
follow the instructions 
1. `cd ~/workspace` ( Always want to cd into workspace so you know where you are )
2. `mkdir first-repo` ( Notice how there are no spaces but instead a dash "-")
3. `cd first-repo` ( Always remember **cd into a file after you make it** )
4. `git init` ( **know where you are before git init** )  
GREAT!  
We now need a remote to push to
**Follow the instructions ** 
1. [Click here](github.com)
2. click on the top right plus icon and create a new repository
3. Repository Name : first-repo
  * THE NAMES ALWAYS NEED TO MATCH!
4. Create Repository 
5. Scroll down to 

Lets make a README now!

**Follow the instructions**
=======
follow the instructions
2. open the README
3. add `this is my first repo`
4. save ( command + s )
5. add 
6. commit -m "create README"



---
### Workflow & Commands
##### Vocabulary 
* **git**: a git command
* **git init** // initializes git in our directory for version control -- **only do this once at the beginning and know where you are.**
* **git add file.ext** // add the file(s) to the stage to be committed (_note: git add . adds the current/entire directory: all files that have changes_) will not add any deleted or rename files
(note: **git add --all  includes ALL changes, including deleted files**)
* **git status** // optional **(recommended!)** command to see which files on the stage are ready to committed (_they will be green if ready if not ready then it will be red_).
* **git commit -m "short/specific message"** // takes a ‘snapshot’ of the files on the stage. The message should be present-tense and short and simple Example: ("Complete first repo")
* **remote**: we are setting up a connection between our current repository and an external one (that lives on github)
* **add**: we are adding the remote repo (as opposed to editing or removing an existing one)
* **origin**: this is our “nickname” for the remote repo.  “origin” is standard.  In the future, you might need multiple remotes.
* **URL**: the location of the remote repo.  (Could be HTTPS or SSH). Recomended that user uses SSH, since HTTPS requires a constant log in after pushing a file.
* **pull**: bring any changes from the remote repo down to the local repo
* **push**: we are sending our commits from our local repo to our remote repo (up to the cloud: Github)
* **-u**: means “upstream.” This tells git to remember which remote repo & branch to push our changes to when we type git push in the future.
---
### Rolling Back Changes
Messed up adding commiting or pushing?

1. Use "git add <file>.." to update what will be commited.
2. Use "git checkout -- <file>..." to discard adding a file to the stage.
3. Use "git reset HEAD <file>..." to unstage.
4. Use "git reset --hard HEAD~1" to nuke the commit.
5. Use "git reset HEAD~1" to undo the commit and keep changes.
6. Use "git reset --soft HEAD~1" to undo your commit but leave your files

---

### Collaberation
With collaboration you can clone or fork repositories.

**Clone**

Cloning is you getting a copy of a repository!

How to clone!
1. Go to the wanted repository/ies 
2. Click the green button `clone or download`
3. Click clone with SSH
4. Click the copy button next to the link.
5. `cd workspace`
6. `git clone <link>`

**Fork**

Forking is you making your own copy of a repository!

How to fork!
1. Go to the repository/ies you want to fork.
2. Click the fork button on the top right.
3. Once you fork check to see if your username replaced theirs 
4. Now you git clone `<link>`.

