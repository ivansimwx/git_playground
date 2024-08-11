# git_playground
# touch test{1..4}.md creates a series of test1 to test4 md files
# git add test1.md && git commit -m 'Create first file'
# git config --global core.editor "code --wait" sets commit message editor to vs code
# git commit --amend does not edit the last commit, it replaces that commit with an entirely new one.
# For example, git rebase -i HEAD~2 allows us to edit the last two commits.

# git rebase -i is a command which allows us to interactively stop after each commit we’re trying to modify, and then make whatever changes we wish. We do have to tell this command which is the last commit we want to edit. For example, git rebase -i HEAD~2 allows us to edit the last two commits.

# Using squash for our commits is a very handy way of keeping our Git history tidy

# When you ran git reset, you reset the current branch by pointing HEAD at the commit right before it. At the same time, git reset also updated the index (the staging area) with the contents of wherever HEAD is now pointed.

# git reset --soft. This would only perform the first part of git reset where the HEAD is moved to point somewhere else but doesnt change the staging area

# it performs all the steps of git reset, moving the HEAD and updating the index, but it also updates the working directory. This is important to note because it can be dangerous as it can potentially destroy data. A hard reset overwrites the files in the working directory to make it look exactly like the staging area of wherever HEAD ends up pointing to.