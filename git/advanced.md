# Advanced Git

Lots of useful little tidbits.

## Setup Git Editor

To specify your default editor, run the following command, replacing `$editorpath`:

```
git config --global core.editor "$editorpath"
```

_Hint: On *nix systems, run `which $faveditor` (where `$faveditor` is your editor of choice) and use that path for `$editorpath`._  
_The following are some examples:_

* nano: `git config --global core.editor "nano"`
* gedit: `git config --global core.editor "gedit -w -s"`

## Branches

Check for any updates

```
git fetch
```

**git branch** - List the current branches on your local repository.

```
git branch
```

**git checkout** - This switches the branch your working on to a different one. Usually it will be to a development branch or a bug fix branch.

```
git checkout dev
```

To add a new branch to your local repository and switch to it.

```
git checkout -b new-branch
```

To delete a local branch. Please make sure you no longer need those file.

```
git branch -d branch-to-delete
```

## Creating Issues

On the GitHub page for the repository click on the issues tab. Then click the green `New Issue` button.

Give an appropriate title and detailed description so people can recreate the issue.

Click Submit New Issue when you're done. A number will be assigned to the issue.

## Closing Issues

In a commit message to that branch include:

```
Fix #X
```

or

```
Close #X
```

## Resources 

- [Git Reset](https://stackoverflow.com/questions/2530060/can-you-explain-what-git-reset-does-in-plain-english#2530073)
- [Git Reset Differences](https://stackoverflow.com/questions/3528245/whats-the-difference-between-git-reset-mixed-soft-and-hard)
- [Git Reflog](http://gitready.com/intermediate/2009/02/09/reflog-your-safety-net.html)
- [How to undo the last commit](https://stackoverflow.com/questions/4114095/how-to-revert-git-repository-to-a-previous-commit)
- [Git Rebase](http://www.jarrodspillers.com/git/2009/08/19/git-merge-vs-git-rebase-avoiding-rebase-hell.html)
- [Git Rebase Info](https://www.linux.com/learn/how-rebase-git)
- [Git Squash](http://gitready.com/advanced/2009/02/10/squashing-commits-with-rebase.html)
- [Making a new repo from an old branch](https://stackoverflow.com/questions/9527999/how-do-i-create-a-new-github-repo-from-a-branch-in-an-existing-repo)
- [Password Caching](https://help.github.com/articles/caching-your-github-password-in-git/#platform)
- [Clean Git History](https://spin.atomicobject.com/2017/04/23/maintain-clean-git-history/) <!-- Maybe not 3, keep all useful commit, not a single feature commit. Look into merge --no-ff instead. Or the below article -->
- [OneFlow Method](http://endoflineblog.com/oneflow-a-git-branching-model-and-workflow)
