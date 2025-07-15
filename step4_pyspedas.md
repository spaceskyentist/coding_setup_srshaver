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
2. Optional: Once it's working you can run:

   ` pip freeze > requirements.txt `

   To lock the environment in case you revisit it later, or want to provide dependencies to other/future users of your project code. 

### Option 2.2: You're given a `requirements.txt` file to install necessary dependencies

## Step 4: Check that it works! (Optional)
1. Create a file in your project to check that PySpedas is working by: **File > New File >** `pyspedas_test.py`, or the little button next to your project name that looks like a piece of paper with a plus sign.
2. Paste this starter code:

   ```
   import pyspedas
   print('yay pyspedas is working!')
    ```
4. Run the Python code by right-clicking in the editor and choose "Run Python File in Terminal", or click the Run ▷ button in the top-right.
5. Yay! It works! (Celebration wiggle). *or* Oh no! It does not work. (Whomp whomp).

## Tips:
- Other packages can be installed and checked in this way
- Some useful packages include `numpy`, `matplotlib`, `pandas`, etc.
