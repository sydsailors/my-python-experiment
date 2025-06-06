# my-python-experiment'
# 01b-create-repo-in-github.md

This page provides instructions to create a new repository in GitHub with a default README file.  
If the repository is created without a README, it will not work the same when cloned. If this happens, delete the repository and start over, ensuring a default README is included.

## Steps to Create a New Repository in GitHub

1. Log in to GitHub. Open your browser and log in to your GitHub account.

2. Go to the "Create Repository" Page  
   - In the top-right corner of GitHub, click the + dropdown menu.  
   - Select New repository.

3. Name Your Repository  
   - Enter a name for your new repository.  
   - IMPORTANT: Follow Naming Guidelines for Python Projects:  
     - Use all lowercase.  
     - Use dashes between words.  
     - NEVER USE spaces or special characters.  
     - Good Examples: my-python-project, python-experiments, baseball-stats, python-personal-project, website-analytics, student-impact-analysis

4. Provide a brief description of your project. This is optional but recommended.

5. Select the `Public` option so others can view your repository. You may always use a fake name.

6. IMPORTANT: Add a Default README File  
   - Check the box for Add a README file. This file is essential for cloning and initializing your project.

7. Click the `Create repository` button to finalize the process and create your repo in GitHub.
# 02-clone-repo-to-local.md

This page provides instructions to copy a GitHub repository to a local machine. 

## Task 1. Copy the Web Address (URL) of Your GitHub Repository

In your browser, view your GitHub repository. 
You should see your account name and the repo name in the browser address bar. 
For example, the URL to this repository (in my account) is <https://github.com/denisecase/pro-analytics-01>.

Verify you are working with a GitHub repository in YOUR account. 
Use `CTRL a` to select all and `CTRL c` to copy the URL to your clipboard. On Mac/Linux, use `CMD a` and CMD c`.


## Task 2. Git Clone the Repo to Your Local Machine

Open a terminal where you keep your GitHub repos (e.g. C:\Repos or ~/Repos). 
On Mac/Linux, use the default Terminal (e.g. zsh or bash), on Windows, use PowerShell. 

In the terminal, type `git clone` leave a single space and use `CTRL v` (or `CMD v`) to paste the URL to your GitHub repository. Hit Enter or Return to run the command. 

The command works in PowerShell, bash, zsh, Git Bash, and more. 
 
```shell
git clone https://github.com/youraccount/yourrepo
```

IMPORTANT: The command is just an example - you must use your GitHub account name and your exact repository name for it to work. 
# 03-add-gitignore-and-requirements.md

This page provides instructions to add common files to a new project repository. 

- `.gitignore` is used to keep things out of GitHub like .venv and secrets
- `requirements.txt` is a good way to list and install external dependencies

## Before Starting

Open your repository in VS Code. 

## Task 1. Create `.gitignore` 

Create a new file in your root repo folder named exactly: `.gitignore`
IMPORTANT: Spelling, capitalization, and name are critical. 
If the name or location is not exact, it will not work. 

Find the `.gitignore` file in the root of this repo and paste the entire contents into your `.gitignore` file.
This is a good starting point for Python projects. 
Actual `.gitignore` contents will vary by project. 


## Task 2. Create `requirements.txt`

Create a new file in your root project folder named exactly: `requirements.txt`.
IMPORTANT: Spelling, capitalization, and name are critical. If the name or location is not exact, the commands we provide will not work. 

Find the `requirements.txt` file in the root of this repo and paste the entire contents into your `requirements.txt`file.
This is a good starting point for Python projects. 
Actual `requirements.txt` contents will vary by project. 
# 04-git-add-commit-push.md

This page provides instructions to add files to version control, commit changes, and push them to your remote repository.

- git add - stages changes, adds files to source control
- git commit - creates a labeled snapshot of staged changes.
- git push - updates the remote repository

## Before Starting

Ensure your project folder is open in VS Code, and you have made changes (e.g. created the .gitignore and requirements.txt files).

## Task 1. Git add-commit-push

Using a terminal in VS Code (PowerShell, zsh, or bash).

IMPORTANT: 
Replace the commit message with a clear and descriptive note about what you added or changed.
Wrap the commit message in double quotes. 

```shell
git add .
git commit -m "Add .gitignore and requirements.txt files"
git push -u origin main
```

After subsequent changes, you may be able to use a simpler version of the last command:

```shell
git push
``` 
# 05-create-virtual-environment.md

This page provides instructions to create a place in your project repository folder that will hold the Python virtual environment for the project. 
It provides an isolated Python environment for the project, so we don't mess up the global Python used by our machine. 

This is typically just done once at the beginning of a project.
If it gets messed up, we can delete .venv and recreate it at any time. 


## Before Starting

Open your project repository in VS Code. 

We'll open a new terminal in VS Code and run a single command to create a new .venv folder for the local project virtual environment.

## Windows Users - Task 1. Create .venv

Run the following command from the project root directory.
 
On Windows, Use PowerShell (not cmd):

```shell
py -m venv .venv
```

## Mac/Linux Users - Task 1. Create .venv

Run the following command from the project root directory.

On Mac/Linux, Use zsh or bash:

```shell
python3 -m venv .venv
```

## Accept VS Code Suggestions

If VS Code asks: We noticed a new environment has been created. 
Do you want to select it for the workspace folder?
Click Yes. 

## **Example Output (Regional Hospitals - NICU Analytics)**
```
---------------------------------------------------------
Regional Hospitals - NICU Analytics
---------------------------------------------------------
Has A Nursery Unit:         True
Years in Operation:         127
Levels Offered:             ['Well-Baby Nursery', 'Special Care Nursery', 'Neonatal Intensive Care Unit', 'Regional Neonatal Intensive Care Unit']
Length of Stay:             [1, 28, 127, 365, 50, 15]
Minimum Length of Stay:     1
Maximum Length of Stay:     365
Mean Length of Stay:        97.67
Standard Deviation of Length of Stay: 138.30
```