<h1 align="center">
📄<br>Git Commands
</h1>

<h1 align="center">
  <img src="github-icon-vector-9.jpg">
</h1>

<p>Git is the open source distributed version control system that facilitates GitHub activities on
your laptop or desktop. This cheat sheet summarizes commonly used Git command line
instructions for quick reference. </p>

## 🚀 Install 

```
https://desktop.github.com/
```

Git distributions for Linux and POSIX systems are available on the official Git SCM web site.

## 🔧 Configure Tooling

Configure user information for all local repositories

Sets the name you want attached to your commit transactions
```
$ git config --global user.name "[name]"
```

Sets the email you want attached to your commit transactions
```
$ git config --global user.email "[email address]"
```

Enables helpful colorization of command line output
```
$ git config --global color.ui auto
```

## ➕ Create Repositories

When starting out with a new repository, you only need to do it
once; either locally, then push to GitHub, or by cloning an
existing repository

Turn an existing directory into a git repository
```
$ git init
```

Clone (download) a repository that already exists on
GitHub, including all of the files, branches, and commits
```
$ git clone [url]
```
## 🌿 Branches

Branches are an important part of working with Git. Any
commits you make will be made on the branch you're currently
“checked out” to. Use `git status` to see which branch that is.

Creates a new branch
```
$ git branch [branch-name]
```
Switches to the specified branch and updates the
working directory
```
$ git checkout [branch-name]
```
Combines the specified branch’s history into the
current branch. This is usually done in pull requests,
but is an important Git operation.
```
$ git merge [branch]
```
Deletes the specified branch
```
$ git branch -d [branch-name]
```

## 🔄 Synchronize changes

Synchronize your local repository with the remote repository on GitHub.com

Downloads all history from the remote tracking branches
```
$ git fetch
```
Combines remote tracking branch into current local branch
```
$ git merge
```
Uploads all local branch commits to GitHub
```
$ git push
```
Updates your current local working branch with all new commits from the corresponding remote branch on GitHub.
`git pull` is a combination of `git fetch` and `git merge` 
```
$ git pull
```

## 🚩 Make changes

Browse and inspect the evolution of project files

Lists version history for the current branch
```
$ git log
```
Lists version history for a file, including renames
```
$ git log --follow [file]
```
Shows content differences between two branches
```
$ git diff [first-branch]...[second-branch]
```
Outputs metadata and content changes of the specified commit 
```
$ git show [commit]
```
Snapshots the file in preparation for versioning
```
$ git add [file]
```
Records file snapshots permanently in version history
```
$ git commit -m "[descriptive message]"
```

<br>[⬆ Back to the top](#git-commands)<br>
