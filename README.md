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

