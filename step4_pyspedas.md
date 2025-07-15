# Install PySPEDAS in your Project Folder

## Step 1: Make sure your virtual environment is activated
1. In your project folder, in VS Code's Terminal, activate your venv:

    ` source my-venv-name/bin/activate `
    
    You should see `(my-venv-name)` in your terminal prompt

## Step 2: Ensure Python Interpreter is the venv interpreter
1. In VS Code, open the command palette (`⇧⌘P`)
2. Type `Python: Select Interpreter`
3. Chose the one with `/your_project/my-venv-name/bin/python`

   You should see `3.xx.xx (my-venv-name)` in bottom right corner of VS Code

## Step 3: Install dependencies for project, like PySPEDAS
### Option 2.1: Do it from scratch
1. Install pyspedas using pip in VS Code's terminal:
     ` pip install pyspedas `

### Option 2.2: You're given a `requirements.txt` file to install necessary dependencies

    
