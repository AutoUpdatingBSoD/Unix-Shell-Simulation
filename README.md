# Unix Shell Simulation

Email me at mhammond9@radford.edu for the source, if you're an employer.

RUSHell 02/26/2018
-------------------------------------------------------------------------------------
GENERAL USAGE NOTES
-------------------------------------------------------------------------------------
- Must be run on a version of Unix (Including, but not limited to Unix Shell on RUCS,
Ubuntu Linux, MacOS X through Unix CMD Tools, and MinGW Windows.
- Windows C++ is not supported for this application.
-------------------------------------------------------------------------------------
Installing Under Versions Listed
-------------------------------------------------------------------------------------
- Type make in the Unix, Linux, or MacOS terminal to compile the program in those Operating Systems
- Use MinGW’s 32-Bit Make to compile the file for Windows in the command line.
- Run ./RUSH example.bin to run the program, where ./RUSH is your executable and example.bin is any file you specify.
-------------------------------------------------------------------------------------
Functionality
-------------------------------------------------------------------------------------
Commands to run in RUSHell:
- pwd : prints the working directory
- ls : calls PWD, but also lists all the files and directories in the current directory.
- createTextFile : Creates an up to 8 alphanumeric character filename with two character extension '.t', and creates its contents.
- mkdir dir : creates an up to 8 alphabetic character directory of name 'dir'
- cd dir : changes to specified directory name 'dir', or if .. is entered changes to the directory above the one you're in.
- cat filename.t : prints a file of name filename and of extension .t
- run progname.p: runs a program of program name 'progname' and of extension '.p'. Prints a statement for now.
- step progname.p: steps a program of program name 'progname' and of extension '.p'. Prints a statement for now.
- starts progname.p: starts a program of program name 'progname' and of extension '.p'. Prints a statement for now.
-------------------------------------------------------------------------------------
Program Information
------------------------------------------------------------------------------------
- RUSH.cpp : contains the functionality that will always be used: The Main Method, the runShell method, and reading and Writing to the directory.
- StringFunctions.cpp : Contains all of the string modification functions. i.e. stripDir().
- BoolFunctions.cpp : contains all of the comparison functions, i.e. checkIfEndDir(), isFile(), containsString(), etc.
- PushFunctions - contains all of the functions that involve pushing items to global stacks. i.e. pushFile(), pushDir(), etc.
- ProgramFunctions.cpp : contains program functions to be used for the next project. Is commented out and not necessary for now.
- PrintFunctions.cpp : contains all of the functions that require printing to the shell not including runShell, but including everything else. i.e. printWorkingDirectory(), listFilesAndDirectories(), printFile()
- OtherFunctions.cpp : contains all of the core functions not in RUSH.cpp and not in PrintFunctions.cpp. i.e. createDir(), changeDirectory()
- GlobalVars.cpp : contains initializations of all Global Variables.
------------------------------------------------------------------------------------- 
