# Installing IDL 

Ahh the Interactive Data Language. Here we go!

https://www.nv5geospatialsoftware.com/Products/IDL

## Step 0: Install XQuartz
XQuartz provided graphical user interface (GUI) capabilities for IDL. XQuartz allows IDL to render and display graphics, such as plots, images, and user interface elements, as noted [here.](https://www.nv5geospatialsoftware.com/Support/Maintenance-Detail/using-idl-and-envi-on-mac-os-x-requires-x11xquartz)

1. [Download XQuartz.](https://www.xquartz.org/) 
2. Unpack and run the XQuartz installer as a user with Admin privileges.  If needed, additional information about installing XQuartz can be found through the XQuartz project web site.
3. Log out and then log back (or reboot) in to complete the XQuartz product installation.

## Step 1: Obtain IDL license
IDL is currently being developed by NV5, so you'll need a license from your institution, research grant, or you can get one yourself [on their website.](https://www.nv5geospatialsoftware.com/Store)

## Step 2: Create an Account
1. Open the portal to [download IDL software.](https://portal.nv5geospatialsoftware.com/auth/sign-in)
2. Next to `Don't have an account?` at the bottom, click the link to Register.
3. Sign up your account.
4. Wait roughly 24 hours for the account to be validated.

## Step 3: Download IDL
1. Open up the login page to [download IDL software.](https://portal.nv5geospatialsoftware.com/auth/sign-in)
2. Download the correct version of IDL for your particular OS

   To know which processing chip you're using on a Mac:

       Click the apple button  at the top left of the screen along the menu bar.
       Click "About this Mac"
       Note the chip, and download IDL accordingly

## Step 4: Install IDL
1. I am following the Mac M-Series instructions from a package, but you can follow the instructions on [IDL's download instructions page](https://www.nv5geospatialsoftware.com/docs/idl-install.html), based on your OS.
2. Open the `.dmg` file you downloaded
3. Follow the GUI installation instructions
4. Choose where you want to install it (e.g., `/Applications/harris` or `/Applications/idl`).
5. When prompted, enter your license information:
     - You can use a **license file** or connect to a **license server.**
     - ⚠️ If you’re using a license server, make sure your network settings allow access to it.

## Step 5: Test Installation
1. Open terminal and run

   ```
   idl
   ```

   Or, if IDL isn't in your path, run:

    ```
   /Applications/NV5/idl/bin/idl
   ```

   Or, if you have an older version, run:
   
   ```
   /Applications/harris/idl/bin/idl
   ```

1. You should see an interactive prompt come up `IDL> `

   You can type:

   ```
   IDL> print, "Hello, world!"
   Hello, world!
   ```
2. Then exit IDL by typing:

   ```
   IDL>exit
   ```
   
## Optional Step 7: Add IDL to your Shell path
To make IDL available in any terminal session:
1. Open your shell config file (`~/.zshrc`, `~/.bash_profile`, or similar):

   ```
   nano ~/.zshrc
   ```

   and/or
   ```
    nano ~/.bash_profile
   ```
   
   
3. Add:
   
   ```
   export PATH="/Applications/NV5/idl/bin:$PATH"
   ```

   Or, if using an older IDL:

   ```
   export PATH="/Applications/harris/idl/bin:$PATH"
   ```

4. Exit nano:
   - Press "Control X" (`⌃X`) to exit
   - Type `Y` to save changes
   - Press enter (`⏎`) to save filename
5. Save and reload
     ```
     source ~/.zshrc
     ```
6. Now, you can run IDL from your terminal by typing:
      ```
      idl
      ```

   exit IDL in terminal by typing

   ```
   IDL> exit
   ```
