# Set up a Project and Virtual Environment (Recommended) 🧑‍💻👩‍💻👾

This instruction guide will help you to create a new project within VS Code, and set up a new virtual environment. If you already have done this and would like to use your previously created project (stored somewhere, e.g., on GitHub), then proceed to step 3: configure Git/GitHub. 

## Step 1: Create Project Folder
1. Open Terminal
2. Create a folder/directory with a name of your choosing:

    `mkdir my-python-project`

    `cd my-python-project `

3. **OR** just create a folder in Finder and open it in VS Code

## Step 2: Open Project in VS Code
1. Open VS Code
2. choose **File > Open Folder**

## Step 3: Create Virtual Environment (Recommended)
1. Open Terminal

   a. Open Terminal from Mac

   b. Open Terminal inside VS Code

       i. Select `Terminal` from top menu bar inside VS Code

       ii. Select `New Terminal` or use `` ⌃⇧` ``
3. Navigate to your project folder (see above)
4. Inside Terminal type

    ` python3 -m venv my-venv-name`
   
   This creates a `my-venv-name/` folder that isolates your project's dependencies (like packages).

## Step 4: Activate the Virtual Environment
1. In terminal, in project folder, run:

   ` source my-venv-name/bin/activate `

   You'll see your terminal prompt change to show ` (my-venv-name) `

## Step 5: Create Project Files
1. Inside your project folder, create:
   - ` main.py ` - Your starting Python script
   - ` requirements.txt ` - list of pip packages (optional for now, but good practice)
   - ` .gitignore ` - if using Git, these are the folders/scripts to ignore in version control syncing (include ` my-venv-name/ `).
2. In VS Code:
   - Click **File > New File** > name it ` main.py `
   - add this test code: ` print("Hello from my project!") `

## Step 6: Select Python Interpreter in VS Code
1. Press `⇧⌘P` or (View > Command Palette).
2. Type: ` Python: Select Interpreter `
3. Choose the one that looks like:

   ` ./my-venv-name/bin/python `

   This ensures VS Code uses the virtual environment's Python.

## Step 7: Install any dependencies
### Option 7.1: Install from scratch
1. To install any packages, type in terminal:

     ` pip install matplotlib`
 2. Then save them to `requirements.txt `:

    ` pip freeze > requirements.txt `

### Option 7.2: Install from a 'requirements.txt' file given to you
     
## Step 8: Run Your Code
1. In VS Code
   - Click the ` ▷Run ` button in the upper right
   - Or right click in the editor **> Run Python File in Terminal**

## Step 9: Deactivate the Environment when Done
1. In Terminal type:

    ` deactivate `
2. To reactivate later:

   ` source my-venv-name/bin/activate `

## ✅ Done!
You now have a clean, isolated Python project set up with:
- A virtual environment
- Your own workspace in VS Code
- Reproducibility for sharing or deployment
