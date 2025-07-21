# IDL Notebooks

## Step 1: Create your first IDL Notebook
1. Click IDL sidebar icon
2. Under "Notebooks" click: `New IDL Notebook`
3. Name your new notebook and save it in your project folder (e.g. 'first_notebook.idlnb`)
4. Now you can mix text and code like Python Notebooks!
5. You can execute different cells one at a time, or run all together.

## Sharing your IDL Notebook
**Note:** ⚠️ IDL Notebooks can only be used by people with IDL for VSCode
If you want to share your Notebook code, you can:
1. Share the Notebook itself to other users who have VSCode
2. Output a PDF of the code
   - Click the PDF button at the top right corner
          <img width="34" height="34" alt="Screenshot 2025-07-21 at 11 36 09 AM" src="https://github.com/user-attachments/assets/4c0bf2ba-c915-4af2-8c25-c89a9310a9c3" />
   - Sometimes you have to click on it twice
   - 
3. Convert the IDL Notebook to PRO Code
   - You can convert your notebook to Pro code, where all the markdown text becomes comments
   - Click the following button, at top right of IDL Notebook screen: <img width="30" height="33" alt="Screenshot 2025-07-21 at 11 54 04 AM" src="https://github.com/user-attachments/assets/c0b82f2a-b5eb-4d25-a6d0-0a5b706378be" />
   - Voila!
   - Any Notebook-environment related functions won't work in PRO code.
        (e.g. `Envi.notebook`, etc.)


## Note: ⚠️ Using Git and saving IDL Notebooks
IDL notebooks are JSON format
1. If using source control, graphics get embedded with source control.
2. **Don't save all of your graphics for source control** otherwise, you'll be saving a HUGE file that may not make it to your version control.
   - Click `Clear all Outputs` at the top of the IDL Notebook before saving your IDL Notebooks to Git/GitHub

