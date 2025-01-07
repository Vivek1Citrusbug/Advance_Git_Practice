# Advance_Git_Practice

--------------------------------------------------------------------
Git Stash Commands : -----------------------------------------------
--------------------------------------------------------------------
git stash push		Save changes to the stash.
git stash push -u	Save tracked and untracked changes.
git stash push -a	Save all changes, including ignored files.
git stash list		View all stashes.
git stash apply		Reapply stashed changes.
git stash pop		Apply and remove the stash.
git stash drop		Delete a specific stash.
git stash clear		Delete all stashes.
git stash branch	Create a branch from a stash.
git stash show		View details of a stash.

--------------------------------------------------------------------
Git rebase Commands : ----------------------------------------------
--------------------------------------------------------------------
- capture all the changes of main branch using pull for upto date 
  information

- then navigate to feature branch

git checkout feature-branch
git rebase main

- if any conflicts then resolve that.

git add .
git rebase --continue

- then all the changes of main will be featured into feature branch.

--------------------------------------------------------------------
Git merge Commands : -----------------------------------------------
--------------------------------------------------------------------

git fetch origin
git checkout your-branch-name
git merge develop
- resolve conflicts if there are any
git push origin your-branch-name

--------------------------------------------------------------------
Git reset Commands : -----------------------------------------------
--------------------------------------------------------------------

rewrites the history so its pretty dangerous.

Command	           Staging Area (Index)	               Working Directory	                         Typical Use Case
git reset --soft	  Keeps all changes staged	          Keeps all changes in working directory	    Undo commit but keep changes staged for a new commit.
git reset --mixed	  Unstages changes	                  Keeps all changes in working directory	    Undo commit and unstage changes for further edits.
git reset --hard	  Resets staging area completely	    Discards all changes in working directory	  Undo commit and completely discard changes.

--------------------------------------------------------------------
Git restore Commands : ---------------------------------------------
--------------------------------------------------------------------

git restore filename     # command used to restore the content of the file to match the content of the last commit 
git restore --staged filename   # remove file from the staging area.

--------------------------------------------------------------------
Git clean Commands : ---------------------------------------------
--------------------------------------------------------------------

git clean -n  # shows untracked files which is going to be removed by this command
git clean -f # removes the untracked files
git clean -f -d # removes untracked directories
