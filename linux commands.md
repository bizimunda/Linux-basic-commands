---------------------------- **File System**---------------------------------------------

#### main list storage
ls /

#### home directory
ls /home 

#### long list of storage
ls l / or ll

#### long list of home
ls -l /home

#### print working directory
pwd

#### change directory
cd

#### binaries or run programs
/bin

#### boot files or boot loader, configuration of your machine
/boot


/etc

blue= folder
white= file
green= program or binary

drwxr
d= directory
-= file
x= execute
l= link

#### root can do anything
---------------------------- **System Log**---------------------------------------------
#### system logs
/var


---------------------------- **File creating**---------------------------------------------


#### create a file
touch fileName

#### to copy file
cp from_file_you_want_to_copy file_to_you_want_to_copy

#### to check if files are not same
diff nameOftheFile nameOftheFile

#### remove files
rm nameOfTheFile
rm -r remove directory and its all sub-directories

#### move files from A to B folder
mv fileName folderName

#### move file to 1 level up
cp nameOfFile ..

#### file permission
drwxrwxr-x
There are in total 3 sections
d=directory
rws= user permision (owner)
rwx= group permission
r-x= everybody else
there sequence never change, always same

#### add permission to the file
chmod + (rwx) nameoffile

#### add permission to the file only for user
chmod u+(rwx) nameoffile

#### add permission to the file for everyone
chmod a+(rwx) nameoffile

#### add permission to the file for group
chmod g+(rwx) nameoffile


---------------------------- **Memory Commands**---------------------------------------------

#### memory commands
free -m

#### disk free (human readable)
df -h

#### disk free inode (capacity of file system to have number of files)
df -i

#### process viewer
htop

#### uptime of your pc
uptime


---------------------------- **Package Managment**---------------------------------------------

#### package managment
update repository
sudo apt update

#### search apt packages
apt search firefox

#### install package
sudo apt install nameofpackage
sudo apt install apache2

#### remove package
sudo apt uninstall nameofpackage
sudo apt autoremove= remove dependent package

#### manage system units
systemctl status nameofpackage
systemctl status apache2

#### to check a specific port
sudo lsof -i:22

#### View logs
different logs have different logs permission

head = first 10 logs
tail = last 10 logs
head -n 50


---------------------------- **Manage Users**---------------------------------------------
### Managing Users

##### to see list of users
cat /etc/passwd
vagrant:x:1000:1000:,,,:/home/vagrant:/bin/bash

x=password (but in another file)
1000 and above are users
under 1000 are systerm users

#### to see hash password
sudo cat /etc/shadow

#### users group
cat /etc/group
groups

#### add user
adduser nameOfUser

#### to see user directory
ll /home

#### login as a specific user
su - nameOfuser

#### login as sudo to a user's directory
sudo su - batman

#### passwd to change that user's password

sudo passw username to change password

#### to login as root 
sudo su -

#### remove a user
sudo userdel -r batman

#### create a group
sudo groupadd nameOfGroup

####adding yourself to a group
sudo usermod -aG nameOfGroup nameOfUser

to check if you are member of a group
groups nameOfUser

#### remove user from a group
gpasswd -d nameOfUser nameOfGroup

#### remove a group
sudo groupdel nameOfGroup




































