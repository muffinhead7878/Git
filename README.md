# Git
Git material
## What is Git?

A free and open source version control system.



## Wt is version control?

The management of changes to documents, computer programs, large web sites, and other collections of information.

Basially a way that w as programmers track our code changes.We basically save an initial version of code into git and then when we update code, we can save it again and again.And throughout the time as our code continues to change, we can look back at all of the changes we have made over time.This helps us to seeand understand wt we did when as well as track dowm our bugs or go back to previous version of our code.



# Terms

directory -> folder

terminal or command line-> interface for text commands

CLI-> command line interface

cd -> change directory ~ same thing as when you double click on folder using the icons on your desktop

code editor -> place to write code

repository -> project or folder/place where your project is kept

git -> is a tool that tracks the changes in your code

github -> is a website where you host all of your git repositories



# Git commands

clone -bring a repo that is hosted somewhere like github into a folder on your local machine

add -> trak youur files and changes in git

commit -> save your files in git

push-> upload git commits to a remote repo, like github

pull -> download changes from remote repo to your local machine, the oppoite of push



## Pull code from github to your VSCode------

go to github-> code -> copy SSH url

open terminal

git bash

git clone <paste copied url>

ls -la-> command to list everything indluding hidden folders or files

make change in code save it

go to terminal

git status -> used to see the files to which the changes are made

git add . ->add all of the files you see in git status

git add <filename> -> add specific file

git status

git commit -m "msg" -m "description"

git commit just saves the code locally

git push -> to push your code changes in github

git push origin master



if you created a new folder or file which is outside the git folder the to add it to get do following steps



git init

git status

git add .

git status

git commit -m "msg"

git push origin master-> throw an error as git not able to recognize where to push this code as theres not connection of it with github

need to create that connection

---

go to github-> create new repo

git remote <ssh url>

git push origin master

if i dont want to type origin master eery time use

git push -u origin master



Github workflow

write code -> commit changes-> make pull request

Local git workflow

write code-> stage changes(git add)->commit changes(git commit)-> push changes(git push)->make a pull request



---------------------------------------------------------------

Git branching



master branch

feature branch





commit1    ->    commit2    ->   commit3    ->    commit4      -> merge



checkout-> used to switch between branches

git branch

git checkout  -b feature_a1 -> creates a new feature_a1 branch and switch from master to feature_a1

git checkout master



git  diff feature_a1 -> show differences

git pull origin master

git branch -d feature_a1 -> to delete the branch

 ---------------------merge conflict------------------------

git checkout -b quick-test

modify file in quick-test branch

git status

git diff

git add .

git commit -am "msg"

git checkout master

modify file in master branch

git checkout quick-test

git status

git commit -am "msg"

git checkout quick-test

git diff master

git merge master --------------gives merge coflict

resolve conflicts in vscode

git diff

git commit -am "msg"

--------------------------Undoing git--------------------------

git reset -> undo staging

git  reset HEAD ~1 -> undo commit

git log -> list of all commits



git reset  --hard 12572376472456458734654->undo all changes upto specific commit

---------------------------------------------------------------------------

Forking-> complete copy of whole repo



click on fork in github select your account 
