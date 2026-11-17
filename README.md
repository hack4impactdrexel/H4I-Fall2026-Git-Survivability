# Git Survivability Workshop

Welcome to **Hack for Impact's Git Survivability Workshop!**

Your goal is to complete eight progressively harder Git challenges using a shared GitHub repository. You'll practice committing, branching, collaborating, recovering from mistakes, and working with multiple Git worktrees.

**The rules are simple:**

- Everyone works in the same shared GitHub repository.
- Complete the challenges in order, at your own pace.
- The contents of your changes don't matter unless a challenge specifies otherwise. Keep them small and harmless.
- **Challenges 1–6** can be verified by a Hack for Impact board member after you've completed them.
- **Challenges 7–8** must be demonstrated live to a board member before they're considered complete.
- Don't delete other participants' branches or intentionally destroy their work.
- If you encounter conflicts or Git errors, figuring them out is part of the challenge!

---

## Challenges

### Challenge 1: First Commit

Make your first contribution to the shared repository.

**Objective:** Get a commit onto the `main` branch with your name as the commit message.

**Completion criteria:**
- Your commit appears on the remote `main` branch.
- The commit message is your name.

### Challenge 2: Branch Out

Time to create your own branch.

**Objective:** Create a new branch following the naming convention `<your-name>/<description>` and make at least one commit on it.

**Completion criteria:**
- Your branch exists on GitHub.
- Your branch contains a commit authored by you.

### Challenge 3: Commit Streak

Now you're working on someone else's branch.

**Objective:** Make three consecutive commits on another participant's branch.

**Completion criteria:**
- The branch belongs to another participant.
- Three consecutive commits authored by you appear in that branch's history.
- All three commits are pushed to GitHub.

### Challenge 4: Request a Review

Practice collaborating through GitHub.

**Objective:** Open a pull request from your branch into `main` and request a review from another participant.

**Completion criteria:**
- Your pull request targets `main`.
- Your pull request includes a brief description.
- You have requested a reviewer.

### Challenge 5: Sync Up

Get your changes merged and synchronize your local repository.

**Objective:** Get your pull request merged into `main`, then update your local `main` branch.

**Completion criteria:**
- Your pull request has been merged on GitHub.
- Your local `main` branch contains the merged changes.

### Challenge 6: Undo Your Mistake

Everybody makes mistakes. Git lets you undo them safely.

**Objective:** Create a commit on your own branch, then revert that commit.

**Completion criteria:**
- Your original commit exists on GitHub.
- A corresponding revert commit exists on the same branch.
- Both commits have been pushed.

### Challenge 7: Stash It Away

Sometimes you need to temporarily save unfinished work without committing it.

**Objective:** Create an uncommitted change, save it in a named stash, switch branches, and restore it.

**Completion criteria:**
- You create a named stash.
- You demonstrate that the changes were temporarily removed from your working directory.
- You switch branches and successfully restore the stashed changes.

**A Hack for Impact board member must observe this challenge live.**

### Challenge 8: Parallel Development

Work on multiple branches simultaneously using Git worktrees.

**Objective:** Create a second working directory using a Git worktree, with a different branch checked out.

**Completion criteria:**
- You have two working directories associated with the same repository.
- Each directory has a different branch checked out.
- You can display both worktrees using Git.

**A Hack for Impact board member must observe this challenge live.**

---

## Git Command Cheat Sheet

Use this reference whenever you get stuck. All the commands and options below are covered in the workshop.

### Getting started

| Command | Description |
|---|---|
| `git clone <url>` | Clone a remote repository |
| `git status` | View modified, staged, and untracked files |

### Staging and committing

| Command | Description |
|---|---|
| `git add <file>` | Stage changes to a specific file |
| `git add <folder>` | Stage changes within a directory |
| `git add .` | Stage changes in the current directory and its subdirectories |
| `git commit -m "message"` | Commit staged changes with a message |

### Remote repositories

| Command | Description |
|---|---|
| `git push` | Push commits to the tracked remote branch |
| `git push -u origin <branch>` | Publish a branch and set its upstream |
| `git pull` | Download and integrate changes from the tracked remote branch |
| `git fetch origin` | Download remote branch information without merging it |

### Branches

| Command | Description |
|---|---|
| `git switch <branch>` | Switch to an existing branch |
| `git switch -c <branch>` | Create a new branch and switch to it |
| `git switch --track origin/<branch>` | Create a local branch tracking an existing remote branch |

**Branch naming convention:** `<your-name>/<description>`

Example: `zach/add-login`

### Commit history and recovery

| Command | Description |
|---|---|
| `git log` | Display commit history |
| `git log --oneline` | Display shortened commit hashes and messages |
| `git revert <commit-hash>` | Create a new commit that reverses an earlier commit |
| `git revert HEAD` | Revert the latest commit |

### Stashing changes

| Command | Description |
|---|---|
| `git stash` | Temporarily save tracked, uncommitted changes |
| `git stash push -m "message"` | Create a named stash |
| `git stash list` | Display saved stashes |
| `git stash pop` | Restore and remove the latest stash |
| `git stash pop 'stash@{n}'` | Restore and remove a specific stash |

### Worktrees

| Command | Description |
|---|---|
| `git worktree add -b <branch> <path>` | Create a new branch in a separate working directory |
| `git worktree list` | List all worktrees |
| `git worktree remove <path>` | Remove a worktree |

### GitHub pull requests

Pull requests are managed through GitHub's website.

- **New pull request:** Propose merging changes from one branch into another.
- **Request review:** Ask another contributor to review your changes.
- **Merge pull request:** Integrate an approved pull request into its target branch.

---

## Good Luck!

Git is one of the most important tools you'll use as a software developer. The best way to learn it is by using it, making mistakes, and figuring out how to recover.

**Interested in building real software for nonprofits?** Ask a Hack for Impact board member how to get involved!