# Revisions and the Cloud

In this assignment I practiced cloning my repository from GitHub.com to my computer using `git clone` command. From then on, I've been editing text in **VSCode** and using **Windows Terminal/Ubuntu** (Terminal) to manage files and directories without having to do it all online on GitHub.

In Terminal I used following commands:

- `mv` to move files from one directory into another and to rename files
- `touch` to create a new file
- `rm -rf` to delete files/directories

After completing the work locally, I uploaded all the changes back to GitHub using an **Add-Commit-Push** prcoess or simply **ACP**.

- ***(A)dd*** to select files to be tracked and staged for committing the changes made 
  - `git add` followed by a file name or `*` to select all files in a repository
- ***(C)ommit*** to commit changes and attaching a message explaining the changes
  - `git commit -m "created TOC, added read01a.md and read03.md, restructured README.md, moved all others into a new 102 folder"`
- ***(P)ush*** upload the changes to GitHub
  - `git push origin main`

In case I don't want to commit changes, but would like to save them anyways, I can use `git stash` command. `git stash apply` command will retrieve those changes should I decide to bring them back.

-----

[<== BACK](102-toc.md)