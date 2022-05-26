1. write your own in a few words on each topic.
2. research using google each topic.
3. revisit - are there a lot of changes?

bonus - FF - fast forward? git merge - signal merge on history
https://youtu.be/LqBC9hSLayc?t=3608

## Git

# Basic commands (init, clone, log, status, add, commit)

[init] - initialises (creates or even wipes out previous git data) on wd.
[clone]- collection of commands (init, pull, remote add) integrates folder and repo
[log]- display the history of previous commits manifesting their sha1,
author, commit etc. from top (current) to bottom (project start)
[status] - display current branch, commit, HEAD but more importantly displays conflicts, detached head status and hints at desired solutions.
[add]- depends on option (for instance . includes files from current dir and -a includes files from the entire workarea) adds changed files.
[commit]- adds a comment on the commit using -m but more importantly creates a point in history, ready to be pushed to remote, indicating file change, code created, a way to "save" current state.
git commit -m -a ?

# Branches Management (checkout, branch)

[checkout]- a command to move between branches, can also create branches or delete them, notice the following slightly confusing commands:
-b: create and change to a new branch
-d: delete a brance - you cannot delet a branch your'e on.
-D: permenently delete a branch

[branch]- show list of branches, using -a show all

# Undoing Changes (revert, reset, cherry-pick)

[revert] a fast way to undo changes, and moving HEAD backword, can be used with ~1 to move backward or ^1 to move deltas/branches
[reset]- not sure, i guess you can move to an older sha1 commit and reset forward changes?
[cherry-pick] a merge between preious states, branches into main branch but selects the files or desired changes and discrds the rest.

# Working with Remotes (fetch, pull, push)

[fetch] retrieve the current repo from origin into the local repo- updates the status of other users as well but does not pull and reflects changes upon working area
[pull] retrieves current commit, origin state from remote into local and the workarea
[push] aftter adding files, commiting changes and not founding conflicts - adds the files into the remote main and advances HEAD

# Merge and Rebase (merge, rebase)

[merge] squash, cherry pick or simply merge all selected branches into the main HEAD as a new commit, solves branches but need to resolve conflicts if there are.
[rebase] - not sure, maybe shifts main into a branch? or moves HEAD from a detached state into a previous commit without opening a new branch?

# gitignore and gitattributes files

[gitignore] prevents "clutter" from being added into the repo (for exmplae vs studio cache files, node_modules and other un-necesary files.)
[gitattributes] dictates repo behaviour, such as no push to main or crlf policy (the difference between line breaks on windows and mac)

# Code Review (Pull Request)

## Scripting Languages

What are scripting languages
What are scripts used for
Variables
Functions
Parameters
Conditions
