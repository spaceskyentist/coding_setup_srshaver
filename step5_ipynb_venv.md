# Enable iPython Notebook in Project's Virtual Environment 📒

## Step 1: Make sure your virtual environment is activated
1. In your project folder, in VS Code's Terminal, activate your venv:

    ` source my-venv-name/bin/activate `
    
    You should see `(my-venv-name)` in your terminal prompt

## Step 2: Install Jupyter and `ipykernel` inside your venv
1. In terminal, run:

   `pip install notebook ipykernel`

    This installs the classic Jupyter Notebook and allows your virtual environment to be used as a kernel.

## Step 3: Register your venv as a Jupyter kernel
1. Give your kernel a custom name (like `my-venv-name`):

   ```
   python -m ipykernel install --user --name=my-venv-name --display-name "Python (my-venv-name)"
   ```

   where:
   - `--name=my-venv-name` is the internal kernel identifier
   - `--display-name "Python (my-venv-name)"` is what you'll see in Jupyter

## Step 4: Start Jupyter Notebook
1. Create an `.ipynb` file in your folder
2. You can now launch Jupyter from your venv in Terminal:

   `jupyter notebook`
3. Navigate to your `.ipynb` file and open it.
4. Under *Kernel* --> *Change Kernel*, select **"Python (my-venv-name)"**.

## ✅ Done!
You're now running notebooks inside your virtual environment with all your installed packages. 
