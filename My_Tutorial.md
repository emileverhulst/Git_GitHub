# Git & GitHub dictionary

## Git

Commit: commit a change to Git every time you make an important change.

GitHub is a kind of timeline of commits.

Changing the past is very dangerous.

The concept of GitHub is similar to google, however google is saving every change for you compared to GitHub when you yourself have to decide when to save/commit changes.

GitHub = Backup of your Timeline.

**Git** = a version control system that lets you manage and keep track of your source code history (**locally**).

**GitHub** = a **cloud-based** hosting service that lets you manage Git repositories.

You can create a new git repository by typing in th the command line: git init

After, by listing the files in the folder where you created the new git repository, you can find a hidden '.git' file.

IMPORTANT: Don't do double git init

IMPORTANT: don't remove the .git folder where your history is kept.

WORDThy do we write commit messages? This message will later on gelp you or anyone else that has access to it; to understand the context of changes and updates.

## Conceptual Areas

1. Development area: working directory

2. Staging area: Temporary space to store file before commiting to the local repo.

3. Local repository is inside the '.git' repository: it is where your snapshots are saved.
   
   1. To access the history in the local repo so I can get information about who, when and what was modified: use <git log>. That will be useful when I want to travel in time.

4. 

Git status allows me to check what files are:

1. To be staged: You have committed this file/folder before, you have made new changes and git recognises the new changes not yet, you have not yet performed add or commit.

2. To be committed: You have committed the file/folder before, you have made new changes and added it to git, but you have not yet committed the file: add but not commit.

3. Untracked: is a completely new file/folder htat has never been add(ed) or commit(ted).

Always check first the status of your files using git status, because you will often not remember anymore which files you have added/committed. Then, add/commit the necessary files always with a meaningful message. If all files are committed, then git will simply say 'nothing to commit, working tree clean'

## GitHub

README.txt or README.md

Overview of what can be found in the repository.

List of files that should not be added to repository:

- Data files

- Backup files

- Intermediate files

-> <.gitignore> 

## Important documents that should be part of my repo

1. README.txt/md: Where I should describe my project, my code, main goals, usage, etc... Can also be a good idea to add links and directions for data that should be related.

2. .gitignore: A text file, without extension that should ALWAYS be in non-caps and where I will list all the files to be ignored and not tracked by git nor shared on github, for example: data files, ...
   
   1. If you include a folder name in the gitignore file, you can also completely ignore a complete folder.

## Connect to remote repository

git remote add <name> <SSH/HTTPS key>

SSH key for Git_GitHub repository = git@github.com:emileverhulst/Git_GitHub.git

Then: git push -> yes.

tralala

HTTPS vs SSH: by using the HTTPS key you should not be able to push/pull or edit the files in the repo, where you should to by using the SSH key.

git branch --list: lists all the branches  that exist and as such if multiple timelines exist.

git checkout <branch_name>:  then you enter the new branch of which you typed in the branch_name.



## Parallel timelines - how to experiment risk free in Git

1. create a new timeline - branch and give it a name
   
   1. 'git branch <name>'

2. checkout to the timeline uou want to work on 
   
   1. 'git checkout <name/id>'

3. 
