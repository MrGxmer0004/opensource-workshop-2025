# Some Extra Terms

Now that you're accustomed to the workflow in Git, let's get to know how to handle some special situations.

## Log

It lists all the commits made in the repository.

`git log` : It shows the commit id and the message along with date,time,user,etc.

`git log --oneline`: It shows the commit id and message in one line.

## Stash

A very useful command used by typing ``git stash`` helps the developer to temporarily store their unsaved work and switch branches. It is analogous to the data structure 'Stack'.

* Why we use it?

    We know commiting a change saves it forever but several commits disturbs the workflow, so we use stash to go to another branch and check any information if needed. 

Few commands related to stash:

``git stash save <name of work>`` : Gives a name to the temporary data to retrieve easily.

``git stash list`` : Lists the works saved in stash.

``git stash apply``: Applies the last work saved in the stash (LIFO: Last In First Out).

``git stash apply stash@{n}`` : Applies the work saved in 'n'th position of the stash.

``git stash pop`` : Applies the last saved temporary work and deletes it from the stash.

Similar to apply I know but apply keeps it in the stash even after applying it to the file.

``git stash drop`` : Deletes the last saved temporary work in the stash.

Can be used for n th position as well like apply.

``git stash clear`` : Cleans/Deletes the entire stash.

## Merge Conflict

When a same file is edited from two branches and then they are merged to the main branch, Git gets confused which one to save. This situation is called a merge conflict.

In VS Code it can be simply solved as it gives us all the permutations and combinations of saving them by just selecting.

Just select and then proceed to add and commit.
