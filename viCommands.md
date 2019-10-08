## Section 1 - Vi Commands

#### Learn more about Vim from the official website [![Image](/images/Vim Logo.jpg)](https://www.vim.org/)

### CD

The **cd** command is used to navigate to different directories. It can be used to go up or down one level (using .. or /) in the directory,or can take the exact location of where we want to go as input and change our directory easily. We use CD to navigate our working directories to access files/locations that are vital to completing the task at hand! We can just use it by writing:
>"cd .." to move UP one directory and "cd /" to move to the root directory.

### MKDIR
The **mkdir** command is used to create a new directory (mkdir is usually followed by the new name of the directory) in the current working directory. We do it when we want to structure the code/files in our project to be organized, so we can find the parts of the code whenever we need to access. The implementation is simple, say we would like to make a directory called testing:
>"mkdir testing" will then create a folder callled testing in our current working directory.

### CP
The **cp** command is used to create a copy from file A to file B. It creates the file in the current directory and is a very straightforward and easy command. For example, if we wanted to create file B as a copy of file A, we could do the following:
>"cp fileA fileB"
It is very very simple to use!

### PWD
The **pwd** commands reports the current working directory path. To use this command, the user only needs to type pwd on a new line and press enter to get the current directory returned. The command goes as follows:
>"pwd"

### MV
The **mv** command will move a file directory, or can be used to rename a file. Make sure that -i is used to not overwrite an existing file. There are a few scenarios in which the mv command can be used.
If you would like to rename a file in the same directory, you would write the following command:
>"mv -i oldFileName newFileName"

If you would like to move a file from a subdirectory to another subdirectory (with both directories being subdirectories of the current directory in this example):
>"mv -i oldSubDirectory/currentFile newSubDirectory"

If we would like to give the moved file a new name, we would do the following:
>"mv -i oldSubDirectory/currentFile newSubDirectory/newFile"

### RM
The **rm** command will remove a file, however -i should be used after typing rm in order to be asked to confirm the file deletion. This is to protect against any accidental file deletions, however it may happen. We do this if we would like to remove any files from within the console, and is a very easy command to use as show below:
>"rm -i randomFile"

In order to remove a non-empty subdirectory, the rm function can accept -r and -f tags that will remove each individual file within the subdirectory. This is different from rmdir because rmdir requests that the subdirectory must be empty. RM -rf will remove the directory and all subdirectory of the specified location:
>"rm -rf oldDirectory"

### History
The **history** command will return the command history since logging into the command line. It is generally used to retrace one's steps and see which commands were used line by line. It is very easy to use this command, since all you need to do is type history as shown below:
>"history"

### Home Directory and File Paths in Linux
When using Unix/Linux, we come across the challenge of having to navigate through multiple directories in order to retrieve the file(s) or complete the tasks required. However, navigating through these paths can become tricky and cumbersome. There are absolute paths and relative paths when we are dealing with file paths, where we use the absolute path name to define the specific location of a file or directory from the root. We use / marks after every directory name in order to navigate through each sublevel of the current working directory. The relative path defines the path related to the present working directory where either a single dot . or double dots .. are used, in conjuncture with **cd** to navigate either up or down levels of the directory.

Here is an example of how these file path concepts are used:  
>__Relative Path example__  
>$pwd  
>/home/test  
>$cd 123  
>/home/test/123  

>__Absolute Path example__  
>$pwd  
>/home/test  
>$cd /home/test/abc/123  
>$pwd  
>/home/test/abc/123  

Read more about Absolute and Relative pathnames [here](https://www.geeksforgeeks.org/absolute-relative-pathnames-unix/)

### Using the Tab key to Complete File Paths
When using the command line, there is a great feature that allows us to type what we want a bit faster. When one or more letters of a file or directory name are filled in, pressing the TAB key will autocomplete the name (in alphabetical order). For example, if we were to type _D_ then press tab, the first directory beginning with the letter _D_ will automatically be typed into the command line. Multiple Tab key presses will allow us to navigate through all available directories in the pwd containing _D_, and this shortcut can be used at any time. The purpose of this shortcut is to save valuable time, where instead of having to go back to get the spelling of a specific directory/file right we can allow the computer to search through the current directory and autocomplete our typing.

### Using the Up and Down arrow for history
As an alternative to the history command, if you would like to print one of the most recent lines of commands that have been executed, it is possible by pressing the up or down arrow  key. The up arrow is used to find the previous relative command, while the down arrow is used to navigate the command list the other way. It is especially effective for when there is an error due to a typing mistake, instead of having to re-write the entire command we can just use the arrows to find the command.

#### Links for Further Reference
[VI and UNIX Quick Reference Sheet](https://acm.cs.virginia.edu/data/viunix.html)  
[Introduction to Unix Commands](https://kb.iu.edu/d/afsk)

## [Click Here to Return to the README](https://github.com/tmccalla777/RBTminiproject--Fall-2019/blob/master/README.md)

