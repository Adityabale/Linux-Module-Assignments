LINUX COMMANDS



----------------------------------------------



System commands



----------------------------------------------



uname/ uname -s

-> returns OS name



uname -r

-> returns OS version/kernel release version



uname -a 

-> returns all system information details including Kernel name, Kernel release and version, Machine hardware name (architecture), Operating system



uname -m

-> returns machine hardware architecture whether 64bit or 32bit



uname -v

-> returns Linux distribution details including built date



uname -n

-> returns hostname



hostnamectl

-> returns details about kernel and hostname. Also includes machine details



cat /etc/os-release

-> returns list of all system variables



hostname -I

-> returns IP address



hostname -f

-> returns qualified domain name



sudo hostnamectl set-hostname <name>

-> will change the hostname



------------------------------------------------



CPU commands



------------------------------------------------



lscpu

-> returns details about CPU

-> to check the resource utilization

-> help with virtualization setup



cat /proc/cpuinfo

-> shows detailed CPU specifications for each core

-> returns details of CPU i.e runtime data of the Cores

-> to check for under utilization or over utilization of the Cores



nproc

-> returns the number of CPUs cores available



---------------------------------------------



Hardware info commands



---------------------------------------------



sudo apt install hwinfo

hwinfo

-> gives detailed information about hardware 



sudo dmidecode -t system

-> returns details about the system



sudo dmidecode -t memory

-> returns details about the memory



sudo dmidecode -t processor

-> returns details about the processor



------------------------------------------------



Memory (RAM) Information Commands



------------------------------------------------



free

-> returns free space available in memory(RAM)



free -h

-> returns free space available in human readable format



cat /proc/meminfo

-> returns detailed memory statistics.



vmstat -s

-> summarizes memory, swap, and paging statistics.

swap refers to a dedicated space on a hard drive or solid-state drive (SSD) that the Linux kernel uses as a temporary overflow for physical RAM. It's an essential part of the system's virtual memory management.



------------------------------------------------



Disk \& Storage Information Commands



------------------------------------------------



df

-> shows disk space usage for all mounted filesystems.



df -h

-> displays disk space usage in human readable format.



lsblk

-> lists block devices (hard drives, SSDs, USBs, partitions) in a tree format.



fdisk -l

-> shows detailed partition table information of all disk



blkid

-> displays UUIDs (Unique IDs) and file system types of partitions.



mount | column -t 

-> lists all mounted file systems, including their mount points and filesystem types.



du -sh /path/to/directory 

-> Displays disk usage of a specific directory.

The -s flag provides a summary of disk usage.

The -h flag makes the output human-readable.



lspci

-> returns information about the peripheral devices Ex. Keyboard, mouse, speakers



lspci -v or lspci -vv

-> shows detailed or very detailed PCI device information.



lsusb

-> returns list of USB devices connected



-------------------------------------------------



Network Information Commands



-------------------------------------------------



ip a/ip addr show

-> shows all network interfaces and their assigned IP addresses.



ifconfig

-> displays network configuration, such as IP address, MAC address, and subnet mask.



ip route

-> displays the kernel's routing table, showing how network traffic is directed.



netstat -r

-> return kernel routing table showing available routes and network gateway information.



ss -tulnp 

->  Shows open ports and active network connections

ss -ta     # Show all TCP connections

ss -ua     # Show all UDP connections

ss -s      # Show summary statistics



hostname -I

-> return system IP address



cat /etc/hosts

-> displays local hostname mappings



ping google.com

-> to tests network connectivity to a specific host.



ip neigh (or arp -a)

-> shows the ARP table (neighbor cache) containing mappings of IP addresses to MAC addresses



nslookup google.com/ dig google.com

-> domain information of the website



traceroute google.com/ tracepath google.com

-> shows the network path that packets take to reach a destination.



-------------------------------------------------



System Uptime \& Load Commands



-------------------------------------------------



uptime

-> displays the system uptime, current time, number of logged-in users, and load average.



top

-> displays real-time CPU and memory usage, along with running processes



last

-> this displays information about the last logged in user with their username, log in time, system shutdown, reboot time and terminal session



htop

-> Interactive process monitoring tool 



vmstat 

-> Monitors CPU, memory, and disk usage every 1 second for 5 times.



sar 

-> System Activity Reporter



dstat 

–> Versatile Resource Monitoring



mpstat 

–> CPU Usage Statistics :mpstat provides detailed CPU statistics, including the usage percentages of each CPU core.



iostat 

–> CPU and I/O Statistics



-------------------------------------------------



User login



-------------------------------------------------



whoami/users

-> this is used to display the current user ID and username of the user who is currently logged in, this will print the username of the user who is running the command.



w

-> current login user and information related to username, log in time, idle time, system load



who

-> this displays information about users who have logged in with their username, terminal session and their log in time



who -q

-> displays only the names and number of users currently logged in



who -r 

-> shows the current run-level of the system



who -a

-> give a comprehensive view of all information about users currently logged in.



who -b 

-> Shows the last system boot time



who -H 

-> Includes column headers in the output



who -u

-> shows the user list with idle time, adding an idle column to the standard display



-----------------------------------------------



Date



-----------------------------------------------



date

-> display Date and Time



date +%y-%m-%d 

-> this displays date in YYYY-MM-DD format



date +%T

-> display time in HHMMSS format



date -u

-> display date according to UTC Time zone



date -u '+%y-%m-%d %H:%M:%S'

-> displays UTC time in a given forma



date '+%A'

-> displays the current day



sudo date +%Y%m%d%H%M.%S -s ‘new date and time’ 

-> This command is used to set new date and time



date +"%H:%M:%S"

-> Displays the current time in the format 12:34:56 (Hour:Minute).



date +"%A, %B %d, %Y"

->Displays a more readable format like Monday, September 04, 2024



--------------------------------------------------



Calander



--------------------------------------------------



cal/ncal

-> display the calendar of a particular year.



cal -y

-> display the calendar for the current year



cal -3 

-> It displays the previous month, current month and next month.



cal -3 2 2020 

-> It displays a calendar for a specific month of the year along with the previous and coming month.



cal -y 2000

-> return calendar for that particular year



cal 2 2003

-> return 2003 feb month calendar



-------------------------------------------------



Accessing File System



-------------------------------------------------



pwd

-> (Print Working Directory) It is used to display the present working directory.



All executable files are stored in bin directory

bin/ls

-> display the version of any command



mkdir <dir name>

-> create new directories



mkdir <dir name1> <dir name2> <dir name3>

-> create multiple directories using command in one single line



cd <dir name>

-> Move into a specific directory



cd ..

-> Move to the parent directory



ls

-> list out all files and directories in current directory.



cd -

-> Move back to the last directory you were in



cd ~

-> Go to your home directory



cd /

-> move to root directory



Cd ~’user’ 

-> go directly to another user's home directory



-------------------------------------------------



Creating Files in Linux



-------------------------------------------------



touch f1.txt

-> create an Empty File



cat t1.txt 

-> show the contents of the file.



echo "hello world, in the next line'> f1.txt

-> add content to the file. It will replace all the text if present



echo "hello world, in line 2">> f1.txt

-> add content to an existing file without overriding the content



printf "hello world, in line 2"> f1.txt

-> create and Update Files. It is similar to echo which creates new files and updates pre-existing files.



nano abb.sh

-> use nano editor to create and open a new file

-> use ctl + x, then type Y and press Enter to save the changes in the file.



bash abb.sh

-> to run/execute the shell file



-------------------------------------------------



Files and directories



-------------------------------------------------



ls 

-> shows a list of files and directories in the current directory.



ls -l 

-> detailed List of Files and Directories



ls -a

-> List All Files, Including Hidden Ones: This will list out all the hidden files (starts with . and ..)



ls -d .\*

-> list out only hidden file



ls -it 

-> List Files Sorted by Modification Date


ls -S 

-> List Files Sorted by Size



ls -n 

-> List Files with Numeric User/Group ID



ls ~ 

-> List Files in the Home Directory: This gives you the list of files and directories at home.



ls \* 

-> This gives you a list of directories and sub directories.



ls -i 

-> List Files with Inodes: This gives you an inode of the directories.

(inode is an index node that is a unique number which holds metadata of file, attributes of file like size, owner of file, creation of file, permission, location, file type and any other link attached to the file).



ls -R 

-> List Files Recursively: This will list you all the directories in tree format



ls -r 

-> List Files in Reverse Order



ls -d \*/ 

-> List Only Directories



ls -l /temp 

-> list of temporary files



ls -IS 

-> List Files Sorted by Size. This gives you a list of files and directories in order of their sizes



--------------------------------------------------



Removing Files and Directories 



--------------------------------------------------



rm ‘filename’ 

-> Remove a Specific File: It is used to remove directories, files and content within the directories.



rmdir ‘directoryname’ 

-> Remove an Empty Directory: Removes the specific directory name.



rm -r ‘directoryname’ 

-> Remove a Directory and Its Contents: This deletes the directory along with its contents



--------------------------------------------------



Copying Files and Directories



--------------------------------------------------



cp ‘source’ ‘destination’ 

-> It is used to copy files and directories from one location to another



cp -n ‘source’ ‘destination’ 

-> Prevent Overwriting Existing Files, does not override an already existing file.



cp -r ‘source’ ‘destination’ 

-> Copy Directories Recursively, copies directories from one place to another.



cp -a  ‘source’ ‘destination’ 

–> Copy and Preserve File Attributes, preserves the file attributes

The -a (archive) option copies files and directories while preserving their attributes, such as permissions, timestamps, and symbolic links.



----------------------------------------------



Moving Files and Directories



----------------------------------------------



mv ‘source’ ‘destination’

-> move file from one location to another

It can also be used to rename files if the destination is a new filename.



mv dir1 ‘destination’ 

-> Move a Directory: This moves the directory.



mv -i test\_report.txt /home/user/backup/

-> mv will overwrite files at the destination without any warning if a file with the same name exists. To avoid this, you can use the -i (interactive) flag, which will prompt you before overwriting



rename ‘s/”old pattern”/ “new pattern”’ “filename to be renamed”

-> We can rename a file using two methods 

S stands for substitute 

/ stands for delimiter used to separate 

g stands for global, if you want to replace all the occurrences globally

^ stands for beginning of the character

$ indicates end of the line 

Example: rename ‘s/\\.txt$/ sh/’ \*txt



rsync 'source' 'destination’

-> It is a command that is used to transfer and synchronize files and directories between two networks, these are specially used to keep backups or to remotely synchronize files



rsync -av ‘source’ ‘destination’ 

-> Sync a Directory Locally with Archive Mode: Sync a directory locally.



Rsync -av -e ssh ‘source’ user@remotehost:’destination’ 

-> Sync Files Remotely Over SSH



----------------------------------------------



Counting Words, Lines, and Characters



----------------------------------------------



wc mozilla.txt

-> return no. of line, no. of words, no. of characters



wc -l mozilla.txt

=> return no. of lines in the file.



wc -w mozilla.txt

-> return the number of words in the file.



wc -m mozilla.txt

-> return the number of characters in the file.



wc -L mozilla.txt

-> return len of longest line in the file.



wc -l \*.txt 

-> Count Lines in Multiple Files



cat file.txt | wc -l 

-> Count the Number of Lines Using Command Sequence



ls | head -n 3

-> return top 3 files in the current directory



ps

-> current process that are running



kill -9 <PID>

-> kill the process matching the process ID



-----------------------------------------------------



Sort command to sort characters and numbers in a file



-----------------------------------------------------



sort example.html

-> sort characters in ascending order



sort -r example.html

-> sort characters in descending order



sort -n example.html

-> sort numbers in ascending order



sort -n -r example.html

-> sort numbers in descending order



sort -n -r -k2 example.html

-> sort based on values in column 2 using -k flag



sort -n -k2 -t $'\\t' -r

-> first access column 2 using k2 flag. Then use delimiter flag -t. To specify tab spacing use $'\\t'



sort -n -k2 -t '|' -r

-> did not use $ sign here since | has only one meaning. (Cross check with chatGPT)



-----------------------------------------------------



Grep – Global Regular Expression Print



-----------------------------------------------------



grep \[options] 'pattern' filename

-> used to search for specific patterns in files. It supports powerful regular expressions, making it ideal for filtering and extracting text.



grep -n ‘pattern’ ‘filename’ 

-> Show line numbers where pattern is matched, returns number of lines where pattern has been found.



grep -c ‘Hello’ ‘filename’

-> Count number of matching lines: Returns number of patterns matched.



grep -v ‘Hello’ ‘filename’ 

-> Show lines that do not match the pattern: Will display number of lines where patterns didn't match.



grep -e ‘Hello’ ‘filename’ 

-> Use expression (for multiple patterns) : Will display matches in case sensitive manner.



grep -i ‘Hello’ ‘filename’ 

-> Case-insensitive match: Will display matches in case insensitive manner.



grep -r ‘Hello’ ‘filename’ 

-> Recursive search in directories : Will find for matches recursively in directories and subdirectories



grep -o ‘Hello’ ‘filename’ 

-> Only show matched pattern, not the entire line: Will display matches without the lines



grep -w "hello" filename.txt 

-> Match the whole word only (not substrings): Matches only lines where "hello" stands as a whole word, not as a part of another word



grep "search\_string" file1.txt file2.txt 

-> Search in multiple files



grep -A 3 "search\_string" 

-> grep -A N — Show N lines After the match: filename.txt shows 3 lines after each match



grep -B 2 "search\_string" filename.txt 

-> grep -B N — Show N lines Before the match: shows 2 lines before each match.



grep -C 1 "search\_string" filename 

-> grep -C N — Show N lines Before \& After match (Context):txt shows 1 line before and after each match.



grep “^H” f1.txt 

-> Match lines starting with H: Show all that matches H at first character grep "^H" filename.txt



------------------------------------------------



Pipe



------------------------------------------------



‘|’ 

-> The | (pipe) in Linux is one of the most powerful tools in the shell.  It is used to connect two commands where one command’s output will act as input for another command.



**Syntax: command1 | command2** 



cat data.txt | grep 'failed' | sort | uniq

-> Chain multiple filters



who | wc -l

-> Count how many users



ps aux | grep java | wc -l

-> Display current processes, filter, and count them



ls -l | grep ^d

-> Show only directories from ls



ls -a ~ | grep ^\\.

-> List only hidden files in the home directory



grep "ERROR" app.log | tail -n 10

-> Show the last 10 error logs from a file



ls -l \*.log | awk '{sum += $5} END {print sum}'

-> Get the total size of .log files



cat words.txt | sort | uniq

-> Sort a word list alphabetically and remove duplicates



ls | wc -l

-> Count the number of files in a directory



ls | sort

-> List all files, sort them alphabetically



grep "success" log.txt | tail -n 5

-> View the last 5 lines of files containing a keyword



history | awk '{print $2}' | sort | uniq -c | sort -nr | head

-> Find most used commands from your history



ls -l | grep ^d

-> List only directories



--------------------------------------------



Common commands



--------------------------------------------



uniq

-> UNIQ is a command-line utility that reports or omits repeated lines



sort sample.txt | uniq

-> Remove all duplicates (sorted output)



sort sample.txt | uniq -d

-> Show only lines that appear more than once



sort sample.txt | uniq -cd

-> Count duplicates only



sort sample.txt | uniq -u

-> Show only lines that appear exactly once



sort sample.txt | uniq -cu

-> Count unique lines



sort mixed\_case.txt | uniq -ci

-> Count case-insensitive



man grep

-> returns details of the command



whatis grep

-> return one line description of the command



mkdir -p a/b/c

-> to create multiple sub-dir



tree a

-> show dir and sub-dir


history

-> show list of last commands used


more f1.txt

-> command is a basic file viewer. It displays the file's content one screen at a time. The command pauses after each screen and shows the percentage of the file you've viewed at the bottom of the terminal.


less f1.txt

-> command is an enhanced version of more. While more is more simplistic and can only move forward in a file, less lets you navigate in both directions, making it more flexible and powerful.


tar -cvf archive_name.tar file1.txt file2.txt

-> The tar command, short for Tape ARchive, is a powerful Linux utility for creating and managing archive files.
-c: create a new archive
-v: verbose, shows the files being added to the archive
-f: specifies the filename of the archive


--------------------------------------------



Zip and unzip commands



--------------------------------------------


zip my_archive.zip file1.txt

-> This command creates my_archive.zip containing file1.txt.


zip my_archive.zip file1.txt file2.txt file3.jpg

-> This command bundles all three specified files into a single zip archive.


zip -r my_archive.zip my_directory/

-> This creates my_archive.zip containing my_directory and everything inside it.


unzip -l my_archive.zip

-> To see what's inside a zip file without extracting its contents, you use the unzip command with the -l (list) option.


zipinfo my_archive.zip

-> The zipinfo command is an alternative that provides more detailed information about the archive's contents, including compression ratios and file permissions.


--------------------------------------------



Replace changes in the file text



--------------------------------------------



sed 's/the/CDAC/' mozilla.txt

-> to replace text 'the' with 'CDAC'

-> does not make changes in the file. Only in the text.



sed 's/the/CDAC/g' mozilla.txt | head -n 10

-> use 'g' at the end for global which means make changes for multiple occurrences in a single line



sed '2d' mozilla.txt | head -n 5

-> d keyword is for delete

-> to remove the 2nd line in the text and showcase only the first 5 lines

-> but changes are only in the text not in the file



sed '$d' mozilla.txt

-> to delete the last line



sed '3,$d' mozilla.txt

-> delete from 3 line to last line



sed '3,7d' mozilla.txt

-> delete range of lines



sed '/the/d' mozilla.txt

-> to delete keyword the from the text



sed '1i\\text\\' mozilla.txt

-> to insert text before the line 1 using 'i'



sed '1a\\text\\' mozilla.txt

-> to insert text after the line 1 using 'a'



-----------------------------------------------------



To find for files and directories using 'find' command



-----------------------------------------------------



find .

-> list out files and directory in current directory



find /home/Aditya -type f

-> list out all files in the directory



find /home/Aditya/ -type d

-> list out all directories with 'd' option



find / mozilla.txt

-> use / to check for file from the root directory



find . mozilla.txt

-> use . to check for file in the current directory



find ~ mozilla.txt

-> use ~ to check for file in the home directory 



find / -type f -atime 1

-> check for files that have been accessed in last one day (1 at the end means day)



find / -type f -mtime 1

-> check for files that have been modified in last one day (1 at the end means day)



find /home/Aditya -type f -perm 777

-> check for files that have permission to read, write and modify



chmod 777 f1.txt

-> change permissions to a file to read, write and modify



find /home/Aditya -type f -size +1K

-> check for files with file size above 1KB



find /home/Aditya -type f -size +1MB

-> check for files with file size above 1MB



find /home/Aditya -type f -empty

-> check for files which are empty



find /home/Aditya -type d -empty

-> check for files dir which are empty



find /home/Aditya -type f -name \*.txt

-> check for files with extension txt



find /home/Aditya -type f -name \*.txt -mtime 1

-> check for files with extension txt that have been modified in the last 1 day.



-------------------------------------------------



locate command to find the path of the file



-------------------------------------------------



locate mozilla.txt 

locate dir1

-> find the path to the file 



locate -r dir1

-> locate the dir and its sub-dir and files. -r stands for recursively means it will search for all files and directories.



locate -i cdac.txt

-> to check for file path ignoring the case using -i flag.



locate -r '\\.txt$'

-> to locate all the files recursively for file extension using regex 



Note: locate is must faster compared to find. Find takes longer time to search for files and directories.





---------------------------------------------------



Creating Hard links (ln) and soft links (ln -s)



---------------------------------------------------



Metadata contains

-> file name

-> file type

-> timestamp

-> permission

-> user/owner



Hard link:



Creating a copy of file sharing the same memory. They both share the same i-node/ID (i-node contains the metadata of the file)

Any changes in original file will reflect the copy file 



ln hardlink.txt copy\_hardlink.txt

-> Will create a copy of new file sharing the same i-node and same ID.



ls -i hardlink.txt copy\_hardlink.txt

-> Since they share the same ID, timestamp in metadata also remain the same.



rm hardlink.txt

-> Even if hardlink.txt file is removed, the copy file will still be there



Soft link:



Creating a copy of file sharing the diff memory. They will have diff i-node/ID 

Any changes in original file will reflect the copy file



ls -n soft.txt copy\_soft.txt

-> create a soft link copy with diff i-nodes



rm soft.txt

ls -li soft.txt

-> if we remove the original file, the copy file will not be accessible and will get deleted.





-------------------------------------------------



Owner and Permissions



-------------------------------------------------



getfacl mozilla.txt

-> returns owner, group names and permissions



setfacl -m u:root:r a.txt

or

setfacl -m user:root:r a.txt

or

setfacl -m g:root:r a.txt

-> changes permissions of the file. (u for user and g for group)



setfacl -b cdac.txt 

-> to restore all the permissions back to original



-------------------------------------------------



Creating new user, groups



-------------------------------------------------



sudo adduser <user-name>

-> create new user, add all the credentials to set up new user.



id <user-name>

-> check user id details.



sudo passwd <user-name>

-> change password for the user



cat /etc/passwd

-> list out all the users



sudo addgroup <group-name>

-> create new group



cat /etc/group

-> to list out all groups



getent group <group-name>

-> check if group is created and list out all the users in the group.



getent passwd <user-name>

-> check if user is created



sudo usermod -aG <group-name> <user-name>

-> add user to a group



sudo useradd -m -G <group-name> <user-name>

-> to create new user and add him in the group.



sudo gpasswd -d <user-name> <group-name> 

-> delete user for the group



sudo userdel <user-name>

-> delete a user



sudo userdel -r <user-name>

-> delete the home directory for the user.



chmod 777 f1.txt

-> change the mode of permissions. 777 mean rwx access to all i.e. user, group, other



chmod u=rx,g=r,o=- cdac.txt

-> custom permissions 



chmod u+w cdac.txt

-> add write permission to the user.



chmod ugo-x cdac.txt

-> to retore permissions to default.



sudo chown <user-name> cdac.txt

-> change owner for a file



sudo chown <user-name> <file-name>

-> change owner for the file



sudo chown <user-name>:<group-name> <file-name>

-> change owner for the group



sudo chown :<group-name> <file-name>

-> retore group owner to <group-name>



sudo chown <user-name>:<group-name> cdac.txt \&\& chmod 777 cdac.txt

-> change username and group for file and also change the permissions.

-> 7-owner, 7-group, 7-other

&nbsp;



-------------------------------------------------------



Shell scripting



-------------------------------------------------------



nano new.sh



\#!/bin/bash                           # this tells the interpreter that it is shell/bash file

echo "hello"



a=20

echo $a



name = "Welcome to cdac"              

echo $name                            # use $ sign to use the variables



read name                             # get user input and assign to variable 'name'

echo "My name is : $name"



bash new.sh                           # to run the shell/bash file



-X--X--X--X--X--X--X--X--X--X--X--X--X--X--X--X-



script1.sh file



readonly ins = "CDAC"

read name 			      # will ask for only name input and not ins





For "readonly" you cannot reassign value but you can use its predefined value.



-X--X--X--X--X--X--X--X--X--X--X--X--X--X--X--X-



script2.sh file



Parameters while running bash file



$0 for file name

$1, $2 for positional parameters

$@ for all parameter values

$# for count of parameters



No space should be provided inbetween spaces



-X--X--X--X--X--X--X--X--X--X--X--X--X--X--X--X-



script3.sh file



sum=$(( $1 + $2 ))

echo $sum



-X--X--X--X--X--X--X--X--X--X--X--X--X--X--X--X-



script4.sh file



read -p "Enter your name" name

echo $name



To print txt before taking input from the user.



------------------------------------------------



SSH server connections



------------------------------------------------



SSH stands for Secure Shell. It is a cryptographic network protocol designed to enable secure communication between two systems over potentially insecure networks. SSH is widely used for remote access to servers and secure file transmission between computers.



Step1: Install ssh package

sudo apt install openssh-server -y



Step2: To start ssh 

sudo systemctl start ssh



Step3: Check status

sudo systemctl status ssh



Step4: To check your IP

hostname -I 



Step5: To connect to a particular system/computer

ssh <user-name>@<IP-address>



You can access all the files and directories within the connected system.



for remote access to servers, use:

ssh user@10.212.00.0 -p 1232





