[Go Back](https://github.com/arm-on/plan/blob/main/README.md)

# Linux Essentials (Next: 21.mp4)

Remember the Goal: Making a list of the most necessary commands to work with linux
| | |
|-|-|
|__command__|__what it does__|
|__General__|
| clear | clear the terminal | 
| history | list all of the commands we executed |
| du -hs /path/to/a/directory/ | see the volume of a directory |
| df -h | see the disk space left for all of the disks |
| nvtop | see the status of the NVIDIA GPU |
| htop | see the status of the CPUs and RAM |
| pwd | show the current directory that the commands are being executed in |
|__HELP__|
| ls --help | documentation of the "ls" command |
| man echo | manual of the "echo" command |
| info echo | more information about the "echo" command (Note: More complete than "man" and "help" commands) |
| whatis ls | what is "ls"? (a very short answer to this) |
|__Audio/Video__|
| ffmpeg -i whatever.webm -c copy whatever.mp4 | convert webm file to mp4 |
|__Working with Files__|
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
| touch test.txt | make a new file named "test.txt" in the current directory |
| nano test.txt | edit the "test.txt" file in terminal |
| cat test.txt | print the content of "test.txt" in the terminal |
| rm test.txt | remove the file "test.txt" |
| rm porteqal.mp4 sound.mp3 linux.png | remove the three files "porteqal.mp4", "sound.mp3", and "linux.png" |
| rmdir /mydirectory/ | remove the directory "mydirectory" (NOTE: works if it's empty) |
| sudo chmod +x myscript.sh | make the script "myscript.sh" executable |
| x=2 | define the variable "x" to be 2 |
| echo $x | print the content of the variable "x" |
| echo "salam" | print the word "salam" |
| echo $a $b | print the content of the variable "a", then a space, and then the content of the variable "b" |
| scp -r speaker* arman@120.233.50.2:~/wavfiles | Copy the folders whose name start with "speaker" from here to the server 120.233.50.2, while logging into that server with the username "arman" |
| cp test.txt /path/to/a/directory | copy the file "test.txt" to a directory |
| cp -r * /path/to/a/directory/ | copy everything inside the current directory (including the folders) to another directory |
| cp -r /first/dir/ /second/dir/ | copy the first directory into the second directory |
| mv test.txt /path/to/a/directory/ | move the file "test.txt" to another directory |
| mv *.txt /path/to/a/directory/ | move all of the files whose name end with ".txt" to another directory |
| mv a.txt b.txt | rename "a.txt" to "b.txt" |
| whereis ls | show the directory in which the "ls" library exists |
| less a.txt | read the contents of a text file one page(one screen) at a time. |
|__Compression__|
| zip media.zip porteqal.mp4 sound.mp3 linux.png | make a zip file containing the tree files "porteqal.mp4", "sound.mp3", and "linux.png". Name the file "media.zip" |
| unzip media.zip | decompress the file "media.zip", and move its contents to the current directory |
| zip linux.zip /path/to/a/directory/ | make a compressed file containing a directory itself (without the files it contains!!!) |
| zip -r tutorial.zip /path/to/a/directory/  | make a compressed file containing a directory and its contents | 
| unzip media.zip /path/to/a/directory/ | decompress the file "media.zip", and move its contents to a desired directory |
| tar -cf myfile.tar porteqal.mp4 sound.mp3 linux.png | "create" a tar "file" (a compressed file with no volume decreasion), given a list of files |
| tar -xf myfile.tar | decompress (extract) a tar file |
| tar -vxf myfile.tar | decompress (extract) a tar file while printing out the things inside it |
| gzip myfile.tar | compress the given "tar" file (which is not volume-efficient) to a .tar.gz compressed file (more compressed than the tar file) |
| gunzip myfile.tar.gz | decompress the .gz file into the .tar file |
| bzip2 myfile.tar | compress the given "tar" file into a .tar.bz2 compressed file (more compressed than "tar") |
| bunzip2 myfile.tar.bz2 | decompress the .bz2 file into the .tar file |
| tar -cvzf media.tgz sound.mp3 porteqal.mp4 | compress some files directly to a tar gzip file (instead of first compressing as "tar", and then "gzip") - Note: "v" stands for "verbose mode" |
| tar -cvjf media.bz2 sound.mp3 porteqal.mp4 | compress some files directly to a tar bzip file (instead of first compressing as "tar", and then "bzip") |
| tar -xvzf media.tgz  | Decompress the .tgz file directly into the original files |
| tar -xvjf media.bz2 | Decompress the .bz2 file directly into the original files |
|__AWS__|
| aws s3 cp /path/to/a/file.txt s3://[bucket-name]/path/to/file.txt --endpoint-url https://[bucket-name].parspack.net | copy a file to a bucket |
| aws s3 cp /path/to/a/folder s3://[bucket-name]/ --recursive --endpoint-url https://[bucket-name].parspack.net | copy a folder to a bucket |
| aws s3 ls s3://[bucket-name]/path/to/a/folder/ -endpoint-url https://[bucket-name].parspack.net | list the contents of a folder |
