# Playground
Sandbox environment for C++ development and 
testing.

If you are unfamiliar with the *markdown* language syntax used in this file, note you can see a friendly rendering of it by clicking on one of the buttons in the upper right corner of VS Code (should say "Open Preview to the Side" when you hover over it). 

To use:
1. Open a terminal window.
2. Navigate to the root of the project folder (e.g., Playground if you took the defaults when you cloned this project from github).  If you are unsure how to navigate in a terminal window, there are many good tutorials on the web.  Quick basics for linux, Mac, or PowerShell:
    - `pwd` will show you what directory you are in
    - `ls` will show you the contents of the current directory
    - `cd <name>` will move you to the directory named "name" in the current directory
    - `cd ..` will take you up one directory to the parent directory
3. If you are on anything other than a native Windows set up (linux, Mac, WSL, remote linux host, or a dev container setup), then use `cmake . -B build` to run CMake.  On a Windows native set up (using MinGW), use the command `cmake . -B build -G "MinGW Makefiles"`.  This will create a new folder named `build` in which it puts a `Makefile` you can use to build your project.
4. Change to the build directory (`cd build`).
5. Run `make` to build the software; if you are on a Windows native set up, you probably need to run `mingw32-make` instead.
6. If there were no compilation errors, then the program `run-main` (or `run-main.exe`) should be in the `build` directory.  You can execute it from the `build` directory using `./run-main`.

This workflow is similar to what we will use in each of the projects in this class; project-specific instructions will be provided with each project.
