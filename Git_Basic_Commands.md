 $ git init :- to initialize the repository

 $ git status :- to view tracked/untracked files

 $ git add . :- to add the files to the staging area

 $ git commit -m "message" :- to push staged files to local repository

 $ git ls-files :- to view the files which are tracking by the git

 $ .gitignore :- create a file .gitignore and add filenames/extensions which you don't want to track

 $ git commit -a -m "message" :- to commit modified files without adding to the staging area

 $ git rm --cached <filename> :- to delete the files in staging area / to untrack the files
 
 $ git reset HEAD filename or git restore --staged filename :- stages files are unstaged
 
 $ git checkout -- index2.html  OR  $ git restore :- permanently delete the changes
 
 $ git revert cid :- file back to the working dir or local repo
