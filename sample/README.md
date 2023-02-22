1. mkdir folder
2. touch README.md
3. git add folder/README.md make the changes you made
4. git commit -m __commitName__
5. git commit -a -m __messageName__ - here this will not create new commit it will add to existing commit

### Staging and Committing ###
Suppose you edited three files (a.md, b.md, and c.md). Now you want to commit all the changes, but you want the changes in a.md and b.md to be a single commit, while the changes to c.md are not logically related to the first two files and should be a separate commit.
1. echo "written to c " > c.md write someting to a,b,c .md files
2. git add a.md, b.md
3. git commit -m "Changes for a and b"
4. git add c.md
5. git commit -m "Unrelated change to c"
6. git reset filename.md To reset stagged files use

### To get back to previous commit ###
1. git log and select first 5 digits for the commit that you want to revert
2. git checkout <5digit>
3. NOTE if you want to commit you have to get back to last commit (you can only see if you want to update you have to create new branch)
4. git checkout main to get back to the last commit
### Undoing comitted changes ###
1. git commit -m "comment"
2. git revert HEAD This will uncommit the last commit
### Creating a branch without conflict ###
1. git checkout -b branchName1 create a branch and checkout to branchName1
2. git status
3. git branch to check where you are in branch
4. add,then commit
5. git push origin branch1 to push to branch1
6. git checkout main
7. git merge branchName1
8. git push
9. git push origin -d branch1 to delete branch for remote
10. git branch --d branch1 to delete branch for local

### Creating a branch without conflict ###
1. git checkout -b branchName1 create a branch and checkout to branchName1
2. git status
3. git branch to check where you are in branch
4. add,then commit
5. git push origin branch1 to push to branch1
6. git checkout main
7. git merge branchName1
8. git push
9. git push origin -d branch1 to delete branch for remote
10. git branch --d branch1 to delete branch for local