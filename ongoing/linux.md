[Go Back](https://github.com/arm-on/plan/blob/main/README.md)

# Linux Essentials (Next: 16.mp4)

Remember the Goal: Making a list of the most necessary commands to work with linux
| | |
|-|-|
|__command__|__what it does__|
| ffmpeg -i whatever.webm -c copy whatever.mp4 | convert webm file to mp4 |
|cd /the/path/of/a/folder/ | change directory |
| cd ~ | change directory to the home dir |
| cd / | change directory to the root dir |
| ls | list the files in the current directory |
|ls -a | list the files in the current directory (including the hidden files) (-a means all) - the files having . at the beginning of their names are hidden |
| ls -l | list the files in the directory with more information (including their read/write access, owner, volume, date&time of creation) |
| ls -la | list ALL of the files in the directory with more information (including their read/write access, owner, volume, date&time of creation) |
| ls /path/to/some/directory/ | list the files in a given directory |
| ls mypattern* | list the files in the current directory with names starting with "mypattern" |
| ls *mypattern | list the files in the current directory with names ending with "mypattern" |
|rm -rf /directory/ | remove everything inside a directory ("r" is for recursive deletion, "f" removes read-only files without asking |
| mkdir directory_name | make a new directory (folder) |
| clear | clear the terminal | 
| touch test.txt | make a new file named "test.txt" in the current directory |
| history | list all of the commands we executed |
| nano test.txt | edit the "test.txt" file in terminal |
| cat test.txt | print the content of "test.txt" in the terminal |
| rm test.txt | remove the file "test.txt" |
| rmdir /mydirectory/ | remove the directory "mydirectory" (NOTE: works if it's empty) |
| sudo chmod +x myscript.sh | make the script "myscript.sh" executable |
| du -hs /path/to/a/directory/ | see the volume of a directory |
| df -h | see the disk space left for all of the disks |
| nvtop | see the status of the NVIDIA GPU |
| htop | see the status of the CPUs and RAM |
| x=2 | define the variable "x" to be 2 |
| echo $x | print the content of the variable "x" |
| echo "salam" | print the word "salam" |
| echo $a $b | print the content of the variable "a", then a space, and then the content of the variable "b" |
| scp -r speaker* arman@120.233.50.2:~/wavfiles | Copy the folders whose name start with "speaker" from here to the server 120.233.50.2, while logging into that server with the username "arman" |
| pwd | show the current directory that the commands are being executed in |
| cp test.txt /path/to/a/directory | copy the file "test.txt" to a directory |
| cp -r * /path/to/a/directory/ | copy everything inside the current directory (including the folders) to another directory |
| cp -r /first/dir/ /second/dir/ | copy the first directory into the second directory |
| mv test.txt /path/to/a/directory/ | move the file "test.txt" to another directory |
| mv *.txt /path/to/a/directory/ | move all of the files whose name end with ".txt" to another directory |
| mv a.txt b.txt | rename "a.txt" to "b.txt" |
| ls --help | documentation of the "ls" command |
| man echo | manual of the "echo" command |
| info echo | more information about the "echo" command (Note: More complete than "man" and "help" commands) |
| whatis ls | what is "ls"? (a very short answer to this) |


