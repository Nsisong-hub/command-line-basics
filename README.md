# Command-Line-Basics
## Project Overview
This project demonstrates essential command-line operations, including directory and file management, copying and deleting files, initializing a Git repository, committing changes, and pushing them to GitHub
## The Directory Structure

`projects/ │── week1/ │ ├── (deleted) hello.txt │── week2/ │ ├── hello_copy.txt │── about_me.txt`


## Step-by-Step Breakdown
**1. Creating Project Directories**
* Create a main directory named `projects`
* Navigates into the projects directory
* Creates two subdirectories: `week1` and `week2`
```bash
mkdir projects
cd projects
mkdir week1 week2
```
<img width="1120" alt="M1" src="https://github.com/user-attachments/assets/56e236ce-d3d2-4497-baa4-5ce228dea6e1" />

**2. Creating a File**
* Navigate into the `week1` directory
* Create an empty file named `hello.txt`
```bash
cd week1

touch hello.txt
```
<img width="1120" alt="M2" src="https://github.com/user-attachments/assets/659a1b9d-90cf-4b00-a78e-c3d0e3f7fc4e" />

**3. Copying the File to Another Directory**
* Move up one directory (back to projects).
* Copy `hello.txt` from `week1` to `week2` with a new name `hello_copy.txt`

```bash
cd ..
cp week1/hello.txt week2/hello_copy.txt
```
<img width="1120" alt="M3" src="https://github.com/user-attachments/assets/23bef66c-4f9f-4007-8de9-186c30e3b629" />

**4. Deleting the Original File**
* Delete `hello.txt` from week1
* `cd` into `week1/`  directory and
* verify that the directory is now empty with `ls` command
  
```bash
rm week1/hello.txt
```

<img width="1097" alt="M4" src="https://github.com/user-attachments/assets/235d7d90-2d92-4988-b6f1-ce36221616c2" />

**5. Writing a Short Paragraph in a Text File Using Vim**
* Open the Vim editor to create or edit about_me.txt
* Press i to enter insert mode
* write a short paragraph about your motivation for learning Node.js
* Press `Esc` to exit INSERT mode.
* Type `:wq` and press Enter to save and exit
  
```bash
 vim about_me.txt
```
<img width="1118" alt="M5" src="https://github.com/user-attachments/assets/223f00b6-b417-4eeb-9d7c-a342b4ab1c1d" />


**6. Initializing a Git Repository**
* Initialize an empty Git repository in the `projects` directory
* Add .DS_Store (macOS system file) to .gitignore to prevent it from being tracked
* Stage all new and modified files for commit
* Commits the changes with a message

```bash
git init
echo ".DS_Store" >> .gitignore
git add .
git commit -m "Initial commit - command line basics assignment"
```
<img width="1120" alt="M6" src="https://github.com/user-attachments/assets/f33a5c96-04a3-463b-b37c-5c54e0877efb" />

**7. Connecting to Remote Repository**
* Link the local repository to a remote
  
```bash
git remote add origin <repo-url>
```
<img width="1021" alt="image" src="https://github.com/user-attachments/assets/c48e56d3-d24f-4723-94dd-3b6ead19e5a0" />

**8. Pushing Changes to GitHub**
* Push the committed changes to the master branch on GitHub

```bash
git push -u origin master
```
<img width="1047" alt="image" src="https://github.com/user-attachments/assets/a84860ea-be69-4236-ae22-988282135cba" />


## Conclusion
This project covers fundamental command-line and Git operations, including creating directories and files, copying and deleting files, setting up Git tracking, and pushing changes to a remote repository.

## Author
* Nsisong Etim
* Contact: [Linkedln](https://www.linkedin.com/in/nsisong-etim-64589126a)
