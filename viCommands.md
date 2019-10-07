Vi Commands!

1. CD

The cd command is used to navigate to different directories. It can be used to go up or down one level (using .. or /) in the directory,or can take the exact location of where we want to go as input and change our directory easily. We use CD to navigate our working directories to access files/locations that are vital to completing the task at hand! We can just use it by writing:
"cd .." to move UP one directory and "cd /" to move to the root directory.

2. MKDIR

The mkdir command is used to create a new directory (mkdir is usually followed by the new name of the directory) in the current working directory. We do it when we want to structure the code/files in our project to be organized, so we can find the parts of the code whenever we need to access. The implementation is simple, say we would like to make a directory called testing:
"mkdir testing" will then create a folder callled testing in our current working directory.

3. CP
The cp command is used to create a copy from file A to file B. It creates the file in the current directory and is a very straightforward and easy command. For example, if we wanted to create file B as a copy of file A, we could do the following:
"cp fileA fileB"
It is very very simple to use!

4. PWD
The pwd commands reports the current working directory path. To use this command, the user only needs to type pwd on a new line and press enter to get the current directory returned. The command goes as follows:
"pwd"

5. MV
The mv command will move a file directory, or can be used to rename a file. Make sure that -i is used to not overwrite an existing file. There are a few scenarios in which the mv command can be used.
If you would like to rename a file in the same directory, you would write the following command:
"mv -i oldFileName newFileName"
If you would like to move a file from a subdirectory to another subdirectory (with both directories being subdirectories of the current directory in this example):
"mv -i oldSubDirectory/currentFile newSubDirectory"
If we would like to give the moved file a new name, we would do the following:
"mv -i oldSubDirectory/currentFile newSubDirectory/newFile"

6. RM
The rm command will remove a file, however -i should be used after typing rm in order to be asked to confirm the file deletion. This is to protect against any accidental file deletions, however it may happen. We do this if we would like to remove any files from within the console, and is a very easy command to use as show below:
"rm -i randomFile"
In order to remove a non-empty subdirectory, the rm function can accept -r and -f tags that will remove each individual file within the subdirectory. This is different from rmdir because rmdir requests that the subdirectory must be empty. RM -rf will remove the directory and all subdirectory of the specified location:
"rm -rf oldDirectory"

7. History
The history command will return the command history since logging into the command line. It is generally used to retrace one's steps and see which commands were used line by line. It is very easy to use this command, since all you need to do is type history as shown below:
"history"
