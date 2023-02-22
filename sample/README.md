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