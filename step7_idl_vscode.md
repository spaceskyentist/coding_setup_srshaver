# Running IDL through VS Code, IDL Notebooks

You can now run IDL through VS Code as they are [offering an extension](https://www.nv5geospatialsoftware.com/Support/Maintenance-Detail/back-to-the-future-idl174-for-visual-studio-code) in the IDE. Even more information can be found:
- [Here for basic info](https://marketplace.visualstudio.com/items?itemName=IDL.idl-for-vscode) 
- [Here for an instruction video](https://www.nv5geospatialsoftware.com/company/events/events-detail/reimagine-the-way-you-program-with-idl-for-vscode)

**Why Use IDL for VSCode?** Well, you can open multiple instances/workspaces of IDL with VS Code, unlike the older IDL workbench. You can compare your IDL code side by side, etc. You can hover over routines, programs, functions, and a popup window will show you how to use the routine. You can copy and paste from these popup windows to start your own code. It's just... better, and more in line with the times. In official language, it's a "modern, user-friendly experience."

In this module, we will go through the steps it takes to download and install IDL for VSCode in VSCode.

⚠️ **Note:** This module assumes you can run IDL from your terminal (i.e., IDL has been added to your PATH). See the previous module on installing IDL for more details.

## Step 1: Open VS Code
You've got this!

## Step 2: Download IDL for VSCode!
1. Navigate to the extensions tab on the left side of VS Code
2. In the searchbar, type, `IDL for VSCode`, and click the install button.

## Step 3: Choose your color theme
1. Under the `IDL for VSCode` extension, click `Set Color Theme`
2. Choose between neon, novus, or retro. You can change this later.
- Retro: eclipse and IDLWorkbench
- Novus: New, dark theme. Similar to other VS Code themes
- Neon: New, dark theme with neon highlighting

## Step 4: Set File Icon Theme
1.  Under the `IDL for VSCode` extension, click `Set File Icon Theme`
2.  Make sure that `IDL (Customized Visual Studio Code)` is selected.

This ensures that your `.pro` programs have an IDL icon next to them so that they're easily recognizable in your folder.

## (Optional) Note: IDL for VSCode reports issues with Code!
1. The color themes will turn your `.pro` files yellow or red if they detect a problem within them (e.g., `unused variable` etc.)
2. If you don't like this then you can change the settings:
- Go to IDL side bar (icon on far left)
- Under quick access, click `Open Extension Settings`, these are the extensions provided by IDL for VSCode
- Select `Problem reporting`
- Scroll to bottom and de-select the option for `Problems: Report Problem`

There ya go!

## (Optional) Settings Configuration:
1. Go to IDL sidebar icon
2. Under quick access, click `Open Extension Settings`, these are the extensions provided by IDL for VSCode
   - General Formatting changes:
      - autoDoc : true/false
        - when formatting code, automatically update documentation
3. **Add Paths** for IDL, adding workspaces to workpath
  - Go to IDL sidebar icon
  - Under quick access, click `Open Extension Settings`
      - Under User/Extensions/IDL for VSCode/IDL
      - You can add in other folders by scrolling all the way to the bottom, and under `idl.IDL:Path` you can click `Add Item` to add paths
        - plus sign before path adds all the folders under a folder
        - get used when you start up IDL debug session, or IDL notebooks

## Step 5: Create a `.pro` file
1. Return to your project folder
2. Create a new file called `hello.pro'
3. In the new file, type:

   ```
   pro hello
   
   print, "Hello, world!"

   end
   ```
  and save file. 

## Step 6: Start up IDL
1. Click IDL sidebar icon!

      <img width="77" height="83" alt="Screenshot 2025-07-21 at 11 03 49 AM" src="https://github.com/user-attachments/assets/42ff56c9-2f46-420e-b4ce-549eadb89652" /> 

3. Under `IDL` click `Start` (a session of IDL)
  - This opens a Debug Console in VS Code, just like in the workbench!
  - Also opens a work bar for running IDL code

      <img width="275" height="48" alt="Screenshot 2025-07-21 at 11 05 27 AM" src="https://github.com/user-attachments/assets/0e495f38-507a-48cc-a35c-0e9266228915" />

## Step 7: Running IDL (2 options)
1. Within the debug console, you can click the run button on the workbar

      <img width="29" height="44" alt="Screenshot 2025-07-21 at 11 07 55 AM" src="https://github.com/user-attachments/assets/8609bd5e-1f59-4741-9e9b-fdc14abdc1f1" />

2. Or go to the embedded Terminal within VSCode (if you don't need the debugger)
   - type `idl` to start idl in Terminal
   - type `hello` to run your "Hello.pro" program







    

