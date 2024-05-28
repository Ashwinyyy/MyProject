# MyProject
# Git Commands Guide

This guide provides a list of common Git commands along with descriptions of what each command does.

## Basic Commands

1. **git init**
   - Initializes a new Git repository.

2. **git status**
   - Shows the working directory status, including staged, unstaged, and untracked files.

3. **git add .**
   - Adds all changes in the working directory to the staging area.

4. **git commit -m "Your commit message"**
   - Commits the staged changes to the repository with a message.

5. **git log**
   - Shows the commit history.

## Remote Repository Commands

6. **git remote add origin <remote-url>**
   - Adds a new remote repository.

7. **git pull origin <branch>**
   - Fetches and merges changes from the remote branch into the current branch.

8. **git fetch origin**
   - Fetches updates from the remote repository without merging.

## Branching and Merging Commands

9. **git checkout -b <branch>**
   - Creates and switches to a new branch.

10. **git merge <branch>**
    - Merges the specified branch into the current branch.

11. **git rebase <base-branch>**
    - Reapplies commits on top of another base tip.

12. **git reset --hard HEAD~1**
    - Resets the current branch to a previous commit, discarding all changes.

## Stashing Changes

13. **git stash**
    - Temporarily saves changes that are not yet ready to commit.

14. **git stash apply**
    - Reapplies the stashed changes.

## Tagging Releases

15. **git tag -a <tag-name> -m "Tag message"**
    - Creates an annotated tag with a message.

## Miscellaneous Commands

16. **git diff**
    - Shows changes between commits, commit and working tree, etc.

17. **git log --oneline**
    - Shows a compact commit history.

18. **git rm <filename>**
    - Removes a file from the working directory and staging area.

19. **git mv <old-filename> <new-filename>**
    - Renames a file and stages the rename.

20. **git cherry-pick <commit-hash>**
    - Applies the changes introduced by some existing commits.

21. **git blame <filename>**
    - Shows who changed each line in a file.

22. **git revert <commit-hash>**
    - Creates a new commit that undoes the changes of the specified commit.

23. **git clean -f**
    - Removes untracked files from the working directory.

24. **git bisect start**
    - Starts a binary search to find a commit that introduced a bug.

25. **git submodule add <repository-url>**
    - Adds a submodule to your repository.

26. **git archive -o <output-file> HEAD**
    - Creates a zip file of the current repository state.

27. **git shortlog**
    - Summarizes git log output by author.

This guide covers a variety of Git commands for initializing repositories, managing changes, working with branches, stashing changes, tagging releases, and more.

