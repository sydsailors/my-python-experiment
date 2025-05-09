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
