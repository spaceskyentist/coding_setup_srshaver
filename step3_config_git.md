# Configuring Git/GitHub in VS Code 😸
Optional, but useful! 

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
1. Create a `.gitignore` file in your project and add:

   ```
   # Ignore Python virtual environment
   my-venv-name/

   # Ignore VS Code settings
   .vscode/

   # Byte-compiled / cache files
   __pycache__/
   *.pyc

   # Ignore system files
   .DS_Store
   ```
     This file tells GitHub what to ignore in your Project folder when commiting messages, perfoming merges, push/pull commands, etc. If you don't do this, you'll likely have *thousands* of commits that can overload these commands!

## Step 4: Stage and Commit your files
1. In Terminal, run the following:

   ```
   git add .
   git commit -m "Initial commit"
   ```

## Step 5: Use VS Code's Git Interface
1. Now that Git is initialized, you'll see source control options in the VS Code sidebar:
   - Click the **Source Control icon*** (third icon from the top or `⌃⇧G`)
   - You'll see your project files listed as changes
   - Type a message in the box (e.g., "Initial commit") and hit the checkmark ✔️ to commit

## Step 6: Conenct to GitHub Repository (Optional, Recommended)
### Option 6.1: If you already have a GitHub repo:
1. In Terminal, run the following:

   ```
   git remote add origin htts://github.com/you-username/your-repo-name.git
   git branch -M main
   git push -u origin main
   ```

You may be prompted to log into GitHub via your browser or VS Code. Do it... or else...

### Option 6.2: If you need to create a GitHub repo:
1. Look it up. I can't do *everything* right now. It's decently straigtforward: [Go to GitHub](https://github.com/)
2. See Option 6.1

## Step 7: Configure Git Username and Email
1. Run these two commands (replacing the info with your own):

   ` git config --global user.name "Firstname Lastname" `

    ` git config --global user.email "your-email@example.com" `
3. ⚠️**Note**: Use the **email associated with your GitHub account** so GitHub links your commits to your profile

    For example, if your GitHub email is `myemail@mail.com`, run:
   
    ` git config --global user.name "myemail@mail.com" `

## Step 8: Re-run the commit command
1. In Terminal in your project folder, in the virtual environment, run:

    ` git commit -m "Merging remote origin/main with local project" `

2. Then push everything from your local device (your computer) to your GitHub repo on the web:

     ` git push `
3. If you want, you can pull everything from the web to your computer, just to be *super certain* everything is matching up:

   ` git pull `

## ✅ Done!
You now have installed git for version control of your code, and have your own repository up and running!
- A virtual environment
- Your own workspace in VS Code
- Reproducibility for sharing or deployment
  
## VS Code Git Tips
- You can **see changes** by clicking on each file in the Source Control panel
- Use **"..." > View >  Commit History** to see Git history
- Press `⌘ShiftP` and type `Git:` to see all available Git commands
