# Configuring Git/GitHub in VS Code (Optional, but useful!)

## Step 1: Download and Install Git
1. Open Terminal and run:
     ` git --version `
2. If it returns something like `git version 2.37.1` then you're good!
3. If not, [install Git for Mac](https://git-scm.com/downloads/mac) and restart VS Code

## Step 2: Initialize Git in your project folder
1. In the Terminal inside VS Code (or regular Terminal if you're in the project folder), run:

   ` git init `

    This creates a `.git` folder, which means your local Git repository is now active!

## Step 3: Create a `.gitignore` File (if you haven't already)
1. 

## Step : Configure Git Username and Email
1. Run these two commands (replacing the info with your own):
    ` git config --global user.name "Space Skyentist" `

    ` git config --global user.email "your-email@example.com" `
2. ⚠️**Note**: Use the **email associated with your GitHub account** so GitHub links your commits to your profile

    For example, if your GitHub email is `myemail@mail.com`, run:
   
    ` git config --global user.name "myemail@mail.com" `

## Step : Re-run the commit command
1. In Terminal in your project folder, in the virtual environment, run:

    ` git commit -m "Merging remote origin/main with local project" `

2. Then:

     ` git push `
   
