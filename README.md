![Git](https://git-scm.com/images/logo@2x.png)

# Why Git?
- Any folder can be a repository.
- Changes can be committed locally, then synced to a remote server any time...or never.
- Branching is easy and robust.
- It's worth learning just because of its extensive community and adoption.
- And it's worth learning the Command line version, especially because it's the most powerful.

# Download and install Git
## Windows
Download and install [Git for Windows](https://git-scm.com/download/win) , which includes the [Git Credential Manager](https://www.visualstudio.com/en-us/docs/git/set-up-credential-managers) to easily connect to Team Services.

## Mac OS X
Use [Homebrew](http://brew.sh/) to install and set up Git.

        brew install git

## Linux and Unix
Use your distribution's package management system to download and install Git. For example, on Ubuntu:

        sudo apt-get install git

Refer to the [list of install commands](https://git-scm.com/download/linux) for the most up to date instructions for your Linux distribution.

# Commands: local
![xkcd Git cartoon](https://imgs.xkcd.com/comics/git.png "xkcd: Git")

## Create a repository
        git init

## View repository changes
        git status

## Add files to a commit
        git add [ * | <file> ]

## Commit changes
        git commit -m "commit message"

## View commit history
        git log
        git log --graph --oneline --decorate --all

## Create a branch
        git branch <branch name>

## Switch to a branch
        git checkout <branch name>
        
## Create and switch to a branch
        git checkout -b <branch name>

## Merge branch-B onto branch-A
        git checkout branch-A
        git merge branch-B

## Discard changes
        git reset --soft                // only moves head within the current branch
        git reset                       // ... also discards staged (tracked) changes
        git reset --hard                // ... also discards unstaged (tracked) changes
        git clean -f                    // discards untracked changes
        
        git reset [ commit | HEAD ]     // reset to a prior commit or offset of HEAD
                
## Discard a commit
        git revert <commit>

# Commands: remote
## Pull changes from the server
        git fetch
        git pull

## Push changes to the server
        git push -u origin <branch name>

# Integration

[Visual Studio](https://www.visualstudio.com/en-us/docs/git/overview)

[VSCode](https://code.visualstudio.com/docs/editor/versioncontrol)

[Eclipse (EGit)](http://www.eclipse.org/egit/)

[IntelliJ](https://www.jetbrains.com/help/idea/2017.1/using-git-integration.html)

# .gitignore
[gitignore.io](https://www.gitignore.io/)

[Java](https://www.gitignore.io/api/java)

[C#](https://www.gitignore.io/api/csharp)

[Angular](https://www.gitignore.io/api/angular)

# Configuration
        git config --global user.name "Gonzo"
        git config --global user.email "gonzo@example.com"
        
        git config --global core.editor ["code" | '"<path to executable>"' ]
Global configuration is located in:  ```%userprofile%\.gitconfig```

# Links
Git documentation:  [https://git-scm.com/docs](https://git-scm.com/docs)

What is Git? (_Visual Studio_):  [https://www.visualstudio.com/learn-git/](https://www.visualstudio.com/learn-git/)

What is Git? (_Atlassian_):  [https://www.atlassian.com/git/tutorials/what-is-git](https://www.atlassian.com/git/tutorials/what-is-git)

Git Tutorial (_Visual Studio_):  [https://www.visualstudio.com/en-us/docs/git/gitquickstart](https://www.visualstudio.com/en-us/docs/git/gitquickstart)

This class:  [https://github.com/aadrew/git-class](https://github.com/aadrew/git-class)


