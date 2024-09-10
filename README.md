# 498 GitHub Lab

### Setting up Git
If you haven't already, install Git on your system 
https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

### Forking a repo
In this exercise, we'll be creating a repo by forking with GitHub. AT the top of this page, find this dialogue by clicking on fork 

![image](https://github.com/user-attachments/assets/5f590784-e375-4332-ac23-b2e0b7f26474)
# 
At the top of your forked repo, check out the options available if you click on 'code' and copy the HTTPS url
#
![image](https://github.com/user-attachments/assets/298afbaa-c194-42b1-86d9-2dbe3f24ce50)

In this lab, we'll be working with git bash. There are other good options such as GitHub Desktop or GitHub's CLI tool

### 1. Cloning a repo
In your local coding environment terminal, navigate to a folder you can clone this repo into and enter ```git clone replace_with_url``` 

In your local environment, edit and fix up the porgram included in the repo. For each change you make, include in a comment above that line what the previous code was or what the issue was

### 2. Pushing and Pulling
#### Using git add
We can add untracked changes/files to gits staging area. These changes will be what get committed when you use git commit. To add a single file ```git add replace_with_file_path``` or add all untracked changes in the repository ```git add .```

#### Using git commit
This will add the changes in your staging area to git's commit history, where git tracks all commits made. You can also revert the most recent commit with ```git reset --soft HEAD~1 ```, or revert a commit with a commit ID using ```git reset replace_with_ID ```. To find a commit's ID, run ```git log``` to view the commit history. Making a commit usually looks like this ```git commit -m "replace_with_message"``` The message you enter will allow you to figure out what each commit did/does. 

#### Using git push
Finally, sending your stuff back to a remote repo is the goal for this lab anyways. The command ```git push origin main``` will automatically push your changes to the remote repo you cloned from. If this project started the other way around, i.e. you made a git repo locally first with ```git init```. Then this command would look like ```git push replace_with_url main``` or you could do ```git remote add origin replace_with_url``` and the first command would work.

### 3. Stuff to note 
#### Code Spaces
While we're here, also check out codespaces. Really simple way to make quick changes or to work without access to your local machine. **HOWEVER** codespace sessions expire, they cannot be saved, without committing changes of course, and there is a usage limit. So this needs to be noted when using codespaces

#### Branching
This is the best way to coordinate multiple people working on the same GitHub project. In your local CLI, the command ```git checkout -b replace_with_branch_name``` will create a new branch or switch to that branch if it already exists. Changes here will not affect main . To merge branches to main, first switch to main ```git checkout main``` and then run ```git merge replace_with_branch_name```. And to push a new branch to the remote repo ```git push origin replace_with_branch_name```

#### Issues and Pull Requests

These are features of GitHub itself. Pull Requests will allow you to merge your repo with a parent repo after forking, or a branch with the main codebase, and can act as a way to review changes as well. It's useful for suggesting changes from a GitHub account without access to the main codebase. 

Issues may alos be useful to us as a way to track bugs and other issues that come up. This is something you should suggest to your clients, if they use GitHub. Internal you can use it for documenting suggestions, managing tasks, or just recording your progress.

### 4. Submission
Include a folder called "submissions" in your new repositories and add screenshots of Task 1 and Task 2.

In Task 1, your screenshot should include the correct output of the program and the command line should show that you are in a git repository

In Task 2, Show in your command line, the commit and push outputs after running the commands.

Finally, make a Pull Request on my repository that you forked from so I can find what you did.
