**Step 1: Folder and Local Repository Creation**



Created the project folder and initialized Git.



cmnds:



git init



**Step 2: Creating Initial Files**



Created the first two required text files(WhatIsGit.txt, BasicCommands.txt)



cmnds:



git add .



git commit -m "Initial commit with task files"



**Step 3-5: GitHub Connection \& Remote Sync**



Connected local repo to GitHub, pushed the main branch, and pulled online edits.



Cmnds:



git remote add origin git@github.com:krishnavijayan34-coder/xminds-training.git



git push -u origin main



git pull origin main



**Step 6: Undo Accidental Add (The Reset)**



Added one.txt and two.txt by mistake and used reset to unstage them.



Cmnds:



git add one.txt two.txt



git reset one.txt two.txt (Unstaged the files successfully)



**Step 7: Branching (Feature Branch)**



Created a new branch for feature development.



Cmnds:



git checkout -b feature1



git add howtobranch.txt



git commit -m "Adding branching file



git push -u origin feature1



**Step 8: Stashing**



Saved work in progress and created a new branch from a specific stash.



Cmnds:



git add fileA.txt fileB.txt



git stash save "Stash 1"



git stash list



git stash apply



git stash save "Second stash - File A updated"



git stash list



git stash branch stash-experiment-branch stash@{1}



**Step 9-10: Pull Request \& Merging**



Added content to files and merged feature1 into main via GitHub.



Cmnds:



git add .



git commit -m "Updated content for Pull request"



git push origin feature1



**Step 9 (Part 2) \& 11: Collaboration \& Conflict Resolution**



Updated friendsBranch and manually resolved a merge conflict in BasicCommands.txt.



Cmnds:



git checkout friendsBranch



git merge main



(Manual Edit in Notepad to fix conflict markers)



git add BasicCommands.txt



git commit -m "Resolved conflict manually"



git push origin friendsBranch



**Step 12: Final Version Tagging**



Created a version tag and pushed it to the remote repository.



Cmnds:



git checkout feature1



git tag -a v1.0.1 -m "Final Submission Version"



git push origin v1.0.1

