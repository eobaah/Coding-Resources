# Git Resources

# Saving/rolling back partial work with git stash

Here’s a good resource on `git stash`: [Atlassian: git stash](https://www.atlassian.com/git/tutorials/git-stash)

I’ve found `git stash` useful in isolated cases, but oftentimes you’ll want to ask yourself “should this just be a new branch instead?” Branching has a lot of advantages.

### Visualizing branches

If you’ve got more than one or two branches, sometimes it can be helpful to visualize them. You can do this on the command line with `git branch` to see the list of branches, and `git log --oneline --decorate --all --graph` to see a pretty visual representation of your branches/commit history.

You can also use a visual GUI to view your repo. I’ve found “SourceTree” by Atlassian to be a good tool for that, though I don’t recommend using it for actually making commits, creating branches etc. Stick to the command line for that.

https://www.sourcetreeapp.com/
Or on homebrew: `brew cask install sourcetree`

### Rolling back uncommited changes

One particularly useful use of `git stash` is when you have a “oh crap. can I just delete everything I’ve done since the last commit?” moment. :facepalm_shake:

To rollback everything you’ve done since your last commit:

`git stash -u` stashes all uncommitted changes, INCLUDING untracked files (files that are new since the last commit, aka not being tracked by git).

Then:
`git stash drop stash@{0}` This is an optional command to delete that last stash. I say it’s optional because you can also just leave the stash there in case you want to come back to it. You’ve already cleared your working directory of the changes you wanted to get rid of. Leaving it there just means you may have a cluttered stash history if you do this more than once.
