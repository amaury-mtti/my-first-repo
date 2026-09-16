Hello essec world.
This is my second line of content.
I don't know what to do.

Answer : 

git status displays readme.txt in red under the heading "Changes not staged for commit". This means Git detects that readme.txt has been modified since the last commit, but the changes have not been added to the staging area yet.

=== Branching & Merging Summary ===

1. Switch back to the main branch:
git switch main

2. List the files in your directory. Is install.sh present? Why or why not?
No, install.sh is not present on main before merging. Git maintains isolation between branches, so files created and committed on feature-script remain exclusive to that branch until merged.

3. What command merges feature-script into main?
git merge feature-script

4. List the files again. What changed?
install.sh is now present in the directory. Merging combined the commit history from feature-script into main and updated the working directory accordingly.

5. Check your commit history. What do you observe?
Running git log displays the commit "Add install script" integrated directly into the commit history of main.

6. What command deletes the feature-script branch after merging?
git branch -d feature-script
