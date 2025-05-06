1. `git init` -> Powers your folder to be managed by git,and initialises a new repository. It also creates a .git folder that has all the relevant logic to maintain versions of your project.

2. `Working area` -> There can be a bunch of files that are not currently handles by git. It means that changes done or to be done in those files are not managed by git yet. A file which is in working area is not considered to be in staging area. When we do git status we see a bunch of `untracked files` then these are actually called to be in the working area.

3. `Staging area` -> What all files are going to be the part of the next verison that we will create.This staging area is the place where git knows what changes will be done from the last version to the next version.

4. `Repository Area` -> This area actually contains the details of all your previous registered version and the files in this area, git already , manages them and knows thier verison history.

5. `git add <file>` -> moves file from working area to staging area.

6. `git rm --cached <file>` -> moves file back form staging area to working area.

7, `commit` -> Commit is a particular version of the project. IIt captures a snapshot of the projects staged changes and creates a verion out of it.

8. `git commit` -> registers staging changes to a commit.

9. `git log` -> list downs all the commmits in the repository. If you want to exit out of git log prompt press 'q'.

10. `git restore <file>` -> it removes all file changes from the staging area to be committed. This can be useful, if we did dirty piece of code and now no more want it. Instead of deleting every change line by line, we can restore it or you can say restore last clean version.

11. `git restore --staged <file>` -> it removes file from the staging area to the working area.
    this only works if changes are in your staging area.

12. Difference between git restore and git rm -> 
    ans : if you want to move the whole file back to the untracked state, then we do git rm, otherwise if we just want the changes to be moved in working area or staging area then we do git restore.
