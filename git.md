# Git Cheat Sheet

## Git vs GitHub

* **Git** = version control software on my computer.
* **GitHub** = stores Git repositories online.

Think:

```text
Git     = notebook
GitHub  = cloud backup
```

---

## My Repository Structure

```text
~/repos
├── learning-notes
└── learning
```

* **learning-notes** → notes (Git, Linux, HTML, CSS, JavaScript)
* **learning** → Odin Project exercises

---

## Creating a New Repository (Odin Method)

1. Create repository on GitHub.
2. Clone it:

```bash
cd ~/repos
git clone git@github.com:USERNAME/REPOSITORY.git
```

3. Enter it:

```bash
cd REPOSITORY
```

`git clone` automatically connects the local repository to GitHub.

---

## Daily Workflow

Check status:

```bash
git status
```

Stage changes:

```bash
git add .
```

Commit:

```bash
git commit -m "Meaningful message"
```

Push to GitHub:

```bash
git push
```

Workflow:

```text
git status
git add .
git commit -m "message"
git push
```

---

## Useful Git Commands

```bash
git status        # Check repository status
git log           # View commit history
git log --oneline # Compact history
git remote -v     # Show connected GitHub repo
git pull          # Download updates
git push          # Upload updates
```

---

## Useful Terminal Commands

```bash
pwd        # Show current folder
ls         # List files/folders
cd folder  # Enter folder
cd ..      # Go up one level
cd ~       # Go home
mkdir name # Create folder
touch file # Create file
code .     # Open current folder in VS Code
```

---

## Important Notes

* `git clone` = download an existing GitHub repository.
* `git init` = create a local Git repository.
* I normally use the Odin workflow: **GitHub → Clone → Work → Commit → Push**.
* I only clone a repository once.
* Most of the time I only need:

```bash
git status
git add .
git commit -m "message"
git push

# Good Git Commit Messages

## Rule

A commit message should clearly describe **what changed**.

---

## Format

Use **imperative mood** (as a command):

```text id="c1"
Add homepage
Fix navigation links
Create images folder
Update README
Remove unused code
```

Think:

> “This commit will… Add / Fix / Create / Update / Remove”

---

## Good Commit Messages

* Add links and images lesson
* Create HTML boilerplate
* Add About page
* Update Git notes
* Fix broken image path
* Move pages into pages directory
* Complete links and images lesson

---

## Bad Commit Messages

Avoid vague messages like:

* update
* changes
* fixed stuff
* done
* work
* new commit

---

## Atomic Commits

Each commit should represent **one logical change**.

Example:

Instead of one big commit:

```text id="c2"
Update website
```

Do separate commits:

```text id="c3"
Add About page
Fix navigation links
Add images
Update README
```

---

## Quick Rule

Before committing, ask:

> “What exactly did I change?”

Then write that as a short action sentence starting with a verb.

```
