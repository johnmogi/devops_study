fast forward
When you try to merge one commit with a commit that can be reached by following the first commit’s history, Git simplifies things by moving the pointer forward because there is no divergent work to merge together – this is called a “fast-forward.”

If Master has not diverged, instead of creating a new commit, git will just point master to the latest commit of the feature branch. This is a “fast forward.”

DELTA - meaning the actual changes on a blob (:
{{  Git uses Delta encoding which indicates a way of storing or transmitting data in the form of differences (deltas) between sequential data ...  }}
blob- {{ This object type is called a blob. You can have Git tell you the object type of any object in Git, given its SHA-1 key, with git cat-file -t }}

## Git

{{ Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency. }}

# Basic commands (init, clone, log, status, add, commit)

[init] -
{{ This command creates an empty Git repository - basically a .git directory with subdirectories for objects , refs/heads , refs/tags , and template files. }}

[clone]-
{{ Clones a repository into a newly created directory, creates remote-tracking branches for each branch in the cloned repository (visible using git branch ... }}

[log]-
{{ This is the default for git log , git show and git whatchanged commands when there is no --pretty , --format , or --oneline option given on the command line. By ... }}

[status]
{{ The git status command displays the state of the working directory and the staging area. It lets you see which changes have been staged, which haven't, and which files aren't being tracked by Git. Status output does not show you any information regarding the committed project history. }}

[add]-
{{ The git add command adds a change in the working directory to the staging area. It tells Git that you want to include updates to a particular file in the next commit. However, git add doesn't really affect the repository in any significant way—changes are not actually recorded until you run git commit . }}

[commit]-
{{ The command git commit -a first looks at your working tree, notices that you have modified hello.c and removed goodbye.c, and performs necessary git add and git ... }}

# Branches Management (checkout, branch)

[checkout]-
{{ Updates files in the working tree to match the version in the index or the specified tree. If no pathspec was given, git checkout will also update HEAD to set ... }}
[branch]-
{{ The git branch command lets you create, list, rename, and delete branches. It doesn't let you switch between branches or put a forked history back together again. For this reason, git branch is tightly integrated with the git checkout and git merge commands. }}

# Undoing Changes (revert, reset, cherry-pick)

did i push or not?

[revert] a fast way to undo changes, and moving HEAD backword, can be used with ~1 to move backward or ^1 to move deltas/branches
!! changes were pushed to remote - now we can revert to go back from our changes !!
{{ Note: git revert is used to record some new commits to reverse the effect of some earlier commits (often only a faulty one). If you want to throw away all ... }}
[reset]- not sure, i guess you can move to an older sha1 commit and reset forward changes?
!! changes were not pushed to remote - we can reset locally !!
{{ You can use git reset to rewind history without changing the contents of your local files, and then successively use git add -p to interactively select which ...
 }}
[cherry-pick]
{[ git cherry-pick is a powerful command that enables arbitrary Git commits to be picked by reference and appended to the current working HEAD. Cherry picking ...
]}

# Working with Remotes (fetch, pull, push)

[fetch] retrieve the current repo from origin into the local repo- updates the status of other users as well but does not pull and reflects changes upon working area
{{ git fetch can fetch from either a single named repository or URL, or from several repositories at once if <group> is given and there is a remotes. }}
[pull] retrieves current commit, origin state from remote into local and the workarea (fetch + merge)
{{ git pull is a Git command used to update the local version of a repository from a remote. It is one of the four commands that prompts network ...  }}
[push] aftter adding files, commiting changes and not founding conflicts - adds the files into the remote main and advances HEAD
{{ git push updates the remote branch with local commits. It is one of the four commands in Git that prompts interaction with the remote repository. }}

# Merge and Rebase (merge, rebase)

[merge] squash, cherry pick or simply merge all selected branches into the main HEAD as a new commit, solves branches but need to resolve conflicts if there are.
{{ git merge ; The "merge" command is used to integrate changes from another branch. ; Creates a merge commit even when a fast-forward would be possible. ; Combines ... }}

[rebase] - not sure, maybe shifts main into a branch? or moves HEAD from a detached state into a previous commit without opening a new branch?
NOPE
rebase merges branch into main but insted of manifesting changes it manipulates the history into a straight line,
for instance, a new branch had 2 commits, by rebasing it shows the 2 new branch commits as a continuation of the main last commit, it actually does so by creating 2 new additional commits for this manipulation...

https://www.atlassian.com/git/tutorials/rewriting-history/git-rebase
Rebasing is the process of moving or combining a sequence of commits to a new base commit. Rebasing is most useful
and easily visualized in the context of a feature branching workflow.
{{ What is git rebase? Rebasing is the process of moving or combining a sequence of commits to a new base commit. Rebasing is most useful and easily visualized in the context of a feature branching workflow. }}

# gitignore and gitattributes files

[gitignore] prevents "clutter" from being added into the repo (for exmplae vs studio cache files, node_modules and other un-necesary files.)
{{ A gitignore file specifies intentionally untracked files that Git should ignore. Files already tracked by Git are not affected; see the NOTES below for ... }}
[gitattributes] dictates repo behaviour, such as no push to main or crlf policy (the difference between line breaks on windows and mac)
{{ A gitattributes file is a simple text file that gives attributes to pathnames. Each line in gitattributes file is of form: pattern attr1 attr2 }}
{{ A gitattributes file is a simple text file that gives attributes to pathnames. Each line in gitattributes file is of form: pattern attr1 attr2 ... That is, a pattern followed by an attributes list, separated by whitespaces. Leading and trailing whitespaces are ignored.
 }}

{{ The . gitattributes file allows you to specify the files and paths attributes that should be used by git when performing git actions, such as git commit , etc. In other words git automatically saves the file according to the attributes specified, every time a file is created or saved.  }}

# Code Review (Pull Request)

merging from a user request to apply changes into main from a different branch
using the ui it's a consideration process, once done the merge is applied.
{{ A pull request – also referred to as a merge request – is an event that takes place in software development when a contributor/developer is ready to begin the process of merging new code changes with the main project repository.
 }}

## Scripting Languages

# What are scripting languages

programming languages for automation and configuration- mainly used for setup purposes
{{ A scripting language or script language is a programming language for a runtime system that automates the execution of tasks that would otherwise be ... }}

# What are scripts used for

"educates" machines for connection as in networks, updates to installations, installations of software, programs, and configuration management tools.
{{ What Does Scripts Mean? Scripts are lists of commands executed by certain programs or scripting engines. They are usually text documents with instructions written using a scripting language. They are used to generate Web pages and to automate computer processes. }}

# Variables

a memory storage unit internally withing a programing or scripting langauge, it stores a memrot of a value- it could be a string, an integar, and other values such as a boolean, a date etc.
a variable can change it's stored data, managing variables within function scopes and checking for value is part of a programmers main tools.
{{ In programming, a variable is a value that can change, depending on conditions or on information passed to the program. Typically, a program consists of instruction s that tell the computer what to do and data that the program uses when it is running. }}

# Functions

methods to be applied within the program are useful to avoid repetetive code and creates cleaner code and structure.
a function is a boxed scoped area in which you either pass parameters and return new values or run other functions, apply commands and calculation etc.
{[ A function is simply a “chunk” of code that you can use over and over again, rather than writing it out multiple times. Functions enable programmers to break down or decompose a problem into smaller chunks, each of which performs a particular task. ]}

# Parameters

a variable that is passed into a function or similiar as an argument to a script file - a function can return a parameter with or without a change.
{{ In computer programming, a parameter or a formal argument is a special kind of variable used in a subroutine to refer to one of the pieces of data provided as input to the subroutine. }}

# Conditions

condition are a set of tools generally applied within an if/ else, while loops, for loops etc, a condition is a value that upon matching either alows the loop to stop or exit, for instance while loop

{{ Conditions are statements that are created by the programmer which evaluates actions in the program and evaluates if it's true or false. If-then-else statement allows conditional execution based on the evaluation of an expression. }}
