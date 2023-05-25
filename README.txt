git init -> powers your folder to be managed by git and initialises a new empty repository. It also creates a .git 
            that has all the relevant logic to manage versions of your project.

Working area -> Bunch of files not handled by git. ie changes done in it are not managed by git. ("Untracked Files")

Staging area -> The files which are going to be part of next version that we'll create. The staging aeea is the place
                where git knows what changes will be done from last version to next version.

Repository area -> This area contains the details of all the previous registered versions, and the files in this area are
                    already tracked by git and git knows their version history.

git add <file> -> adds file from Working area to staging area.

git rm --cached <file> -> removes file from staging area to Working area.

commit -> it is a particular version of the project, it captures a snapshot of projects staged changes and creates a 
            version out of it.

git commit -> registers staging changes to a commit.

git log -> list down all the commits of the repository.

git restore <file> -> it removes all file changes from staging area to be commited. This can be useful if we did dirty
                    piece of code and no more want it.

git restore --staged <file> -> it removes file changes from staging area to Working area. This only works when changes
                are in your staging area.

diff b/w rm and restore -> it you want to move whole file back to Untracked area, do git rm otherwise if we want  the 
                        changes to be moved from working area or staging area then we do git restore.

