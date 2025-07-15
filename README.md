# coding_setup_srshaver
This repository contains a step-by-step guide to setting up coding software on your **Mac**. 

Step 1: [Install VS Code and Python](https://github.com/spaceskyentist/coding_setup_srshaver/blob/76bab996c8380504de6eb52cf532b68df50aa5ce/step1_install_vscode_python.md)


# Getting VSCode and Python Up and Running 🏃‍♀🏃‍♂💨

## Step 1: Download and Install VSCode
1. Go to the VS Code website: [vscode](https://code.visualstudio.com)
2. Click the "Download for Mac" button (make sure it says "Universal" or matches your chip, like Intel or Apple Silicon/M1/M2/M3
3. Once the '.zip' file downloads, double-click it to extract and open the Visual Studio Code app.
4. Move VS Code to Applications folder: Drag it into your Applications folder for easy access.

## Step 2: Install Python
1. Go to the official Python website: [python](https://www.python.org/downloads)
2. Click "Download Python 3.x.x" (the latest stable version).
3. Open the '.pkg' file once downloaded and go through the installer steps.
4. After installation, open Terminal (you can search for it via Spotlight), and type:

    `python3 -- version`

You should see something like 'Python 3.12.3' (or whichever version you installed).

## Step 3: Add Python Extension in VS Code
1. Open VS Code
2. Click the **Extensions icon** on the sidebar (or press `⇧⌘X`).
3. In the search bar, type **Python** and install the official one from **Microsoft**
4. Once installed, it will help with syntax highlighting, linting, running Python files, etc.

## Step 4: Set Python Interpreter in VS Code
1. Open a Python file (or create a new one with '.py' extension).
2. In the bottom-left corner, you’ll see `Python x.x.x.` Click it.
3. Choose the interpreter that says something like:

   `/usr/local/bin/python3`
   
## Step 5: Run Python Code
1. Create a file like `hello.py`
2. Write:

    `print("Hello, world!")`

3. Right-click in the editor and choose "Run Python File in Terminal", or click the play button in the top-right.
4. Yay! It works! (Celebration wiggle).

## ✅ Done!
You have now: 
- Downloaded and installed VS Code
- Downloaded and installed Python on your computer
- Set up Python in VS Code
- Ran your very first python code!

# Set up a Project and Virtual Environment (Recommended) 🧑‍💻👩‍💻👾

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
