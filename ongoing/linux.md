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