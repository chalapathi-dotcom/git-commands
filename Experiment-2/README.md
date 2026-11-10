# Experiment II – Git Commands

## Aim
Demonstrate the following Git commands with examples:
1. Pull
2. Clone
3. Checkout

## 1. Git Clone
**Meaning:** Clone downloads an entire remote GitHub repository to the local computer.

Open Git Bash and run:

```bash
cd D:
git clone https://github.com/chalapathi-dotcom/git-commands.git
cd git-commands
ls
```

The repository is downloaded to the local system. The `ls` command displays the files.

## 2. Git Pull
**Meaning:** Pull downloads the latest changes from the remote repository and integrates them into the current local branch.

First, add or edit a file in the GitHub repository and commit the change. Then run:

```bash
git pull origin main
ls
```

The latest remote changes are downloaded and integrated into the local `main` branch.

## 3. Git Checkout
**Meaning:** Checkout is used to switch between branches or restore files from a previous commit.

Check the current branch:

```bash
git branch
```

Create a new branch named `testing`:

```bash
git branch testing
```

Switch to the new branch:

```bash
git checkout testing
```

Create a file in the testing branch:

```bash
echo "This is testing branch" > test.txt
```

Stage and commit the file:

```bash
git add test.txt
git commit -m "Added test file"
```

Switch back to the main branch:

```bash
git checkout main
git branch
```

The asterisk (*) indicates the currently active branch.

## Final Verification

Run the following commands to verify the repository status, branches, and commit history:

```bash
git status
git branch
git log --oneline
```

## Result
Successfully demonstrated the Git commands Clone, Pull, and Checkout. The repository was cloned, remote changes were pulled, and a new branch was created, switched, and used to commit a file.

---
**Repository:** https://github.com/chalapathi-dotcom/git-commands
