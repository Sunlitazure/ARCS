# ARCS: Azure Robotics Control System

## Repo Setup
- Download the wxwidgets source code to a temp folder: https://www.wxwidgets.org/downloads/
- Build and install wxWidgets using instructions from https://wiki.wxwidgets.org/Compiling_and_getting_started for Linux/OSX or https://wiki.wxwidgets.org/Compiling_wxWidgets_with_MinGW for windows
- For windows, download and install MinGW: https://osdn.net/projects/mingw/releases/
    - Download the .exe
	- once installed run the MinGW Installer it creates
	    - install the mingw32-base-bin, mingw32-gcc-g++-bin, and both MSYS items
		- Installation -> apply changes
		- -> apply
		- C:\MinGW\msys\1.0 -> copy msys.bat to desktop. This will be used to compile programs
		- add C:\MingW\bin and C:\MinGW\libexec\gcc\mingw32\8.2.0 to user variable "PATH" in System Properties -> Environment Variables
		
## Compile
- compile example code:
    - go to C:\wxWidgets-3.1.2\examples\minimal
		- use either mingw32-make.exe -f makefile.gcc or in MSYS make -f makefile.gcc
		- https://stackoverflow.com/questions/15713244/compiling-a-wxwidgets-application-with-mingw-from-prompt-under-windows-xp
		
## Custom makefile
- use make -f makefile.gcc -n on the "minimal" sample. Make your own makefile using the commands that lists