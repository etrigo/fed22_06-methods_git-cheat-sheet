# Git Cheat Sheet

_I´l bet you have a laugh at this project. But you said we could select technologies our selfs and the important thing is the git history. I´m ~~building~~ writing a short Git cheat sheet to brush up on my markdown and to read up on Git at the same time._

### git-init

**Create a new repository:**

```
$ git init
```

_This will create a new empty repository._
[Read more](https://git-scm.com/docs/git-init)

### git-log

**See what happened:**

```
$ git log
```

_This will show commit logs. You can type "q" to exit git log and return to command prompt_

```
$ git log --oneline
```

_This will show commit logs in one line per log._
[Read more](https://git-scm.com/docs/git-log)

### git-switch

**Switch branches:**

```
$ git switch <branch>
```

_This will switch branch._

[Read more](https://git-scm.com/docs/git-switch)

### git-checkout

**Switches branches:**

```
$ git checkout <branch>
```

_This will switch (checkout) branch._

```
$ git checkout -b <new-branch>
```

_This will create a new branch and switch (checkout) to it._

[Read more](https://git-scm.com/docs/git-checkout)

### git-branch

**List, create or delete branches:**

```
$ git branch
```

_This will list all branches in the repository._

```
$ git branch -v
```

_This will list all branches in the repository with additional information._

```
$ git branch -r
```

_This will list all branches in the remote repository._

```
$ git branch -a
```

_This will list all branches in the repository including remotes._

```
$ git branch -r -v
```

_This will list all branches in the remote repository with additional information._

```
$ git branch -a -v
```

_This will list all branches in the repository including remotes with additional information._

```
$ git branch <new-branch>
```

_This will will create a new branch from the current branch._

```
$ git branch -d <branch>
```

_This will will delete a branch from the repositiory._

[Read more](https://git-scm.com/docs/git-branch)

### git-add

**Add file contents to the index:**

```
$ git add *
```

_This will add all visible files._

```
$ git add .
```

_This will add visible files._

```
$ git add <file>
```

or

```
$ git add index.html
```

_This will add specific file._

```
$ git add <folder>
```

or

```
$ git add src/
```

_This will add specific folder._

this will not be added

[Read more](https://git-scm.com/docs/git-add)

### git-status

**Show the working tree status:**

```
$ git status
```

_This will show current status._

```
$ git status -b
```

_This will show the branch and current status._

```
$ git status -b -s
```

_This will show the branch and current status in short format._

[Read more](https://git-scm.com/docs/git-status)

### git-commit

**Record changes to the repository:**

```
$ git commit -m "A commit message"
```

_This will record modifications with a commit message._

[Read more](https://git-scm.com/docs/git-commit)

### git-merge

**Join two or more development histories together:**

```
$ git commit <branch>
```

_This will merge the selected branch in to the currently checked out branch._

[Read more](https://git-scm.com/docs/git-merge)

### git-rebase

**Reapply commits on top of another base tip:**

```
$ git rebase <branch>
```

_This will automatcilly perform a "git switch <branch>" before anything else. Then it will merge the changes on the before checked out branch ontop of the now checked out branch._

[Read more about rebase vs merge](./rebase-vs-merge.md)
[Read more](https://git-scm.com/docs/git-rebase)

### git-cherry-pick

**Apply the changes introduced by some existing commits:**

```
$ git cherry-pick <commit>
```

_This will apply selected commit into the checked out branch._

[Read more](https://git-scm.com/docs/git-cherry-pick)
