Git Commands
============

## Translated Versions
- [Versão em português](READMEpt.md)
- [Versión en español](READMEes.md)
- [Türkçe versiyon](READMEtr.md)
- [বাংলা সংস্করণ](READMEbn.md)
- [हिन्दी अनुवाद](READMEhi.md)
- [العربية](READMEar.md)

---

*A list of commonly used Git commands from basic to advanced*

### Getting & Creating Projects
| Command | Description |
| ------- | ----------- |
| `git init` | Initialize a local Git repository |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | Create a local copy of a remote repository |
| `git clone [url]` | Clone a repository using HTTPS or SSH |

### Basic Snapshotting
| Command | Description |
| ------- | ----------- |
| `git status` | Check status |
| `git add [file-name.txt]` | Add a file to the staging area |
| `git add -A` | Add all new and changed files to the staging area |
| `git commit -m "[commit message]"` | Commit changes |
| `git commit -am "[commit message]"` | Add and commit in one step |
| `git rm [file-name.txt]` | Remove a file |
| `git rm -r [file-name.txt]` | Remove a file (or folder) |
| `git mv [old-file-name.txt] [new-file-name.txt]` | Rename a file |

### Branching & Merging
| Command | Description |
| ------- | ----------- |
| `git branch` | List branches (the asterisk denotes the current branch) |
| `git branch -a` | List all branches (local and remote) |
| `git branch [branch name]` | Create a new branch |
| `git branch -d [branch name]` | Delete a branch |
| `git branch -D [branch name]` | Force delete a branch |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git checkout -b [branch name]` | Create a new branch and switch to it |
| `git checkout [branch name]` | Switch to a branch |
| `git checkout -` | Switch to the branch last checked out |
| `git checkout -- [file-name.txt]` | Discard changes to a file |
| `git merge [branch name]` | Merge a branch into the active branch |
| `git merge --no-ff [branch name]` | Merge a branch into the active branch with a merge commit |
| `git stash` | Stash changes in a dirty working directory |
| `git stash list` | List stashed changes |
| `git stash apply` | Apply the latest stashed changes |
| `git stash apply stash@{n}` | Apply specific stashed changes |
| `git stash clear` | Remove all stashed entries |

### Sharing & Updating Projects
| Command | Description |
| ------- | ----------- |
| `git push origin [branch name]` | Push a branch to your remote repository |
| `git push -u origin [branch name]` | Push changes to remote repository (and remember the branch) |
| `git push` | Push changes to remote repository (remembered branch) |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git pull` | Update local repository to the newest commit |
| `git pull origin [branch name]` | Pull changes from remote repository |
| `git fetch` | Fetch all branches from remote repository |
| `git fetch origin` | Fetch all branches from remote repository |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Add a remote repository |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Set a repository's origin branch to SSH |

### Inspection & Comparison
| Command | Description |
| ------- | ----------- |
| `git log` | View changes |
| `git log --summary` | View changes (detailed) |
| `git log --oneline` | View changes (briefly) |
| `git log --graph --oneline` | View changes as a graph |
| `git diff` | Show changes between commits, commit and working tree, etc. |
| `git diff [source branch] [target branch]` | Preview changes before merging |
| `git diff --staged` | Show changes between staged changes and the last commit |
| `git show [commit]` | Show various objects (blobs, trees, commits, tags) |
| `git blame [file]` | Show what revision and author last modified each line of a file |

### Advanced Commands
| Command | Description |
| ------- | ----------- |
| `git rebase [branch]` | Reapply commits on top of another base tip |
| `git rebase -i [commit]` | Start an interactive rebase |
| `git cherry-pick [commit]` | Apply the changes introduced by some existing commits |
| `git revert [commit]` | Revert a commit by making a new commit |
| `git reset [commit]` | Reset your current branch to a specific commit |
| `git reset --hard [commit]` | Reset and discard all changes to a specific commit |
| `git reset --soft [commit]` | Reset to a specific commit, but keep changes staged |
| `git reflog` | Show a log of changes to the local repository's HEAD |
| `git clean -f` | Remove untracked files from the working tree |
| `git clean -fd` | Remove untracked files and directories |
| `git bisect start` | Start a binary search to find a commit that introduced a bug |
| `git bisect bad` | Mark the current commit as bad |
| `git bisect good [commit]` | Mark a known good commit |
