<img width="468" height="14" alt="image" src="https://github.com/user-attachments/assets/c229918c-6bdd-462b-b29a-61bac94171e2" /># IDL Packages
Where to find SPEDAS, NASA CDF Routines, SPICE, etc. 

# SPEDAS
[SPEDAS Wiki.]{https://spedas.org/wiki/index.php?title=Downloads_and_Installation}

# SPICE
[SPICE toolkit.]{http://naif.jpl.nasa.gov/naif/toolkit.html}

[SPICE tutorials.]{http://naif.jpl.nasa.gov/naif/tutorials.html}


NASA's SPICE toolkit, provided by the Navigation and Ancillary Information Facility (NAIF). Best known use is for satellite ephemeris data, reference frames, etc.

## SPICE for IDL - Icy
### Step 1: Download Icy SPICE
1. Navigate to the SPICE toolkit page: [SPICE toolkit.]{http://naif.jpl.nasa.gov/naif/toolkit.html}
   - SPICE for IDL is called 'Icy'
2. Select the operating system you are running on. I'm a Mac user.
   - **NOTE:** If you have an ARM MacOS (with an M-series chip), there has been compatibility issues with Icy.
   - A development version of N0067-based Icy is in the works and can be found [here.]{https://naif.jpl.nasa.gov/pub/naif/misc/toolkit_dev/N0067/IDL/MacM1_OSX_clang_64bit/}
   - You may have to go to your privacy and security settings to allow icy.so to be run after Step 3 is completed.
4. Save the .tar.z or .zip file to any directory. I put mine near my IDL code.
5. Uncompress the file you just saved.

### Step 2: Copy files to your IDL dlm Directory
1. Determine your IDL dlm directory
   - Open an IDL terminal
   - type `print, !DLM_PATH` into the IDL terminal
   - This is where the IDL dlm directory can be found for the following step:
2. Copy and paste the binary and dlm files from the package you unzipped in Step 1 to your IDL dlm directory. These are typically found in the icy/lib folder.
  - The dlm file is called `icy.dlm`
  - The binary file name is different depending on your OS. For Windows it is `icy.dll`, on linux, unix, and MacOS it is called `icy.so`

### Step 3: Restart IDL
1. Restart IDL
2. You can check that the icy routines are incorporated by typing `help, 'icy',/dlm` into the IDL terminal
   - You should see some info about SPICE like:

     ```
      ** ICY - IDL/CSPICE interface from JPL/NAIF (not loaded)
      Version: 1.9.0, Build Date: 05-NOV-2021, Source: Marc.Costa.Sitja@jpl.nasa.gov
      Path: /Applications/NV5/idl91/bin/bin.darwin.arm64/icy.so
     ```
3. Congrats, SPICE is installed!


## SPICE for IDL - Icy for MacOS Mseries chip!
There has been some issues getting SPICE to run with the ARM Macs, or those with an M Chip.
A development version of N0067-based Icy is in the works and can be found [here.]{https://naif.jpl.nasa.gov/pub/naif/misc/toolkit_dev/N0067/IDL/MacM1_OSX_clang_64bit/}



