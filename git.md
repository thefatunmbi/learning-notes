# Git Cheat Sheet

## Configure Git

git config --global user.name "David Fatunmbi"

* Set my commit author name.

---

git config --global user.email "my-noreply-email"

* Set my commit email.

---

git config --global --list

* View Git settings.

---

## Repository Basics

git init

* Create a new Git repository.

---

git clone URL

* Download a repository from GitHub.

Example:
git clone https://github.com/user/project.git

---

## Checking Status

git status

* Show changed, staged, and untracked files.

This is the command I should use most often.

---

## Staging Files

git add file.txt

* Stage one file.

---

git add .

* Stage all changes.

---

## Committing

git commit -m "message"

* Save a snapshot of staged changes.

Example:
git commit -m "Add homepage"

---

## Viewing History

git log

* Show commit history.

---

git log --oneline

* Compact commit history.

---

## GitHub

git remote -v

* Show connected GitHub repository.

---

git push origin main

* Upload commits to GitHub.

Think:
push = local → GitHub

---

git pull origin main

* Download updates from GitHub.

Think:
pull = GitHub → local

---

## Typical Workflow

1. git status
2. git add .
3. git commit -m "Describe changes"
4. git push origin main

Repeat every time I finish a piece of work.



One more thing to jot down

Git vs GitHub

Git = version control software on your computer.
GitHub = website that stores Git repositories online. GitHub

Think of it like:

Git     = notebook
GitHub  = cloud backup for the notebook

---

git clone means

"Make a copy of a Git repository from somewhere else onto my computer."

Think of it as downloading a project with its entire Git history.

Example

Suppose you have a repository on GitHub:

https://github.com/thefatunmbi/learning-notes

You can copy it to your computer with:

git clone https://github.com/thefatunmbi/learning-notes.git