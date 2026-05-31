# Command Line Basics Cheat Sheet

## Navigation

pwd

* Print Working Directory
* Shows where I currently am.

Example:
pwd
Output:
/home/david/projects

---

ls

* List files and folders in the current directory.

Examples:
ls      -> list files
ls -a   -> show hidden files
ls -l   -> detailed view

---

cd foldername

* Change directory.
* Move into a folder.

Example:
cd projects

---

cd ..

* Move up one directory.

Example:
/home/david/projects
↑
cd ..
↓
/home/david

---

cd ~

* Go to my home directory.

---

## Special Symbols

.

* Current directory.

Examples:
code .
ls .
cp file.txt .

---

..

* Parent directory (one level up).
Example:
cd ..

---

~

* Home directory.

Example:
cd ~

---

*

- Wildcard (matches anything).

Example:
*.txt = all text files

---

## Creating Files and Folders

mkdir foldername

* Create a folder.

Example:
mkdir my-project

---

touch filename

* Create an empty file.

Example:
touch index.html

---

## Copying Files

cp source destination

* Copy a file.

Example:
cp index.html backup.html

---

cp -r folder1 folder2

* Copy a folder and everything inside it.

---

## Moving and Renaming

mv oldname newname

* Rename a file.

Example:
mv file.txt notes.txt

---

mv file folder/

* Move a file into another folder.

Example:
mv file.txt Documents/

---

## Deleting

rm filename

* Delete a file.

Example:
rm file.txt

---

rmdir foldername

* Delete an empty folder.

---

rm -r foldername

* Delete a folder and everything inside.

---

rm -i filename

* Ask for confirmation before deleting.

---

## Viewing File Contents

cat file.txt

* Display file contents.

---

less file.txt

* View a long file page by page.

Press q to quit.

---

## Helpful VS Code Command

code .

* Open the current folder in VS Code.
