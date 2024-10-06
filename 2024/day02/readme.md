## Basic linux commands

### Listing commands
```ls option_flag arguments ```--> list the sub directories and files avaiable in the present directory

Examples:

- ``` ls -l ```--> list the files and directories in long list format with extra information
- ```ls -a ```--> list all including hidden files and directory
- ```ls *.sh``` --> list all the files having .sh extension.

- ```ls -i ``` --> list the files and directories with index numbers inodes
- ``` ls -d */``` --> list only directories.(we can also specify a pattern)

### Directoy commands
- ```pwd``` --> print work directory. Gives the present working directory.

- ```cd path_to_directory``` --> change directory to the provided path

- ```cd ~ ``` or just  ```cd ``` --> change directory to the home directory

- ``` cd - ``` --> Go to the last working directory.

- ``` cd ..``` --> change directory to one step back.

- ``` cd ../..``` --> Change directory to 2 levels back.

- ``` mkdir  directoryName``` --> to make a directory in a specific location

Examples:
```
mkdir newFolder              # make a new folder 'newFolder'

mkdir .NewFolder              # make a hidden directory (also . before a file to make it hidden)

mkdir A B C D                  #make multiple directories at the same time

mkdir /home/user/Mydirectory   # make a new folder in a specific location

mkdir -p  A/B/C/D              # make a nested directory
```

Madhav notes

What is Linux?
Linux is an operating system or a kernel distributed under an open-source license.
The kernel is the heart of the Linux operating system, responsible for managing communication between hardware and software.

Benefits of Linux
Free to use: Linux is completely free and open-source.
Open and Complete: You can view and modify the source code to suit your needs.
Continuously Improved: A large community of developers constantly enhances it.
Zero-Downtime Patching: It offers the ability to patch the kernel without needing reboots.
Cloud-Ready: It serves as the foundation for many cloud-native tools.
Secure: Known for its stability and security.

Popular Linux Distributions
Red Hat Enterprise Linux
Fedora
Debian
Linux Mint
Ubuntu Linux
Basics of Linux Commands
Linux commands form the backbone of system navigation and file management. Let’s explore some key ones:

pwd: Shows the current directory you are in. The output is the absolute path starting from the root.
history: Displays a list of previously executed commands in the terminal.
man & - -help: Used to display the manual of any command.
cd: Change the current directory. For example, if you want to go to the Downloads folder, use the command cd downloads.
rm: Removes files or directories. To remove directories and their contents, use rm -r.
touch: Creates a new, empty file.
cp: Copies files from one location to another. It takes two arguments: the source file and the destination.
mv: Moves files or renames them.
locate: Helps to find files by name, similar to the search function in Windows.
Listing Commands
The ls command helps you list files and directories within your current working directory.

ls -al: Shows all files, including hidden ones.
ls -l: Lists files in a long format, including details like file size, permissions, and modification date.
ls -a: Lists all files, including hidden ones.
ls -lh: Displays file sizes in human-readable format.
ls -d */: Displays only directories.

Working with Nested Directories
The mkdir command allows you to create directories and subdirectories.

mkdir folderName: Creates a single directory.
mkdir .NewFolder: Creates a hidden directory by prefixing the folder name with a dot.
mkdir A B C: Creates multiple directories at once.
mkdir -p A/B/C/D: Creates nested directories in one go.