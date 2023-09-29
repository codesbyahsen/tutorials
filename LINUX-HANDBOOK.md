# Linux Handbook
Introduction to the linux commands. In this guide, you will learn Linux shell commands and their functionalities.
<br/> <br/>


## Table of Contents
- [What is Linux?](#what-is-linux)
- [Basic Commands](#basic-commands)
- [Environment Variables](#environment-variables)
- [Package Installation](#package-installation)
- [Install .deb Packages](#install-deb-packages)
- [Remove Packages](#remove-packages)
- [Remove .deb Packages](#remove-deb-packages)
- [Update Packages List](#update-packages-list)
- [Upgrade Installed Packages](#upgrade-installed-packages)


## **What is Linux?**
Similar to Windows and macOS, Linux functions as an operating system. Linux represents a collection of open-source Unix-like operating systems, which are founded upon the Linux kernel. This kernel was initially introduced by Linus Torvalds on September 17, 1991.
<br/><br/>


### **Basic Commands**
Allows regular users to run programs with the security privileges of the superuser or root
```
sudo
```
<br/>

Command used to install and update packages
```
apt-get
```
<br/>

Or
```
apt
```
<br/>

Show all files and directories(folder)
```
ls
```
<br/>

Show sub-directories as well
```
ls -R
```
<br/>

Show hidden files as well
```
ls -a
```
<br/>

Show all files and directories with detail information
```
ls -al
```
<br/>

Navigate to `Home` directory
```
cd
```
<br/>

Or
```
cd ~
```
<br/>

Move one step level up
```
cd ..
```
<br/>

Move two step level up
```
cd ../..
```
<br/>

Move to `root` directory
```
cd /
```
<br/>

Create a new file
```
cat > filename
```
<br/>

Show the content of the file
```
cat filename
```
<br/>

Delete file
```
rm filename
```
<br/>

Gives a list of all past commands typed in the current terminal session
```
history
```
<br/>

Clears the terminal
```
clear
```
<br/>

Create new directory
```
mkdir directoryname
```
<br/>

Delete directory
```
rmdir directoryname
```
<br/>

To show file type and access permission
```
ls -l
```
<br/>

(r) - Read <br/>
(w) - Write <br/>
(x) - Execute <br/><br/>
Permission Read, Write, Execute for all
```
chmod 777
```
<br/>

Permission rwx for owner, rx for group and world
```
chmod 755
```
<br/> <br/>


### **Environment Variables**
Displays all environment variables
```
env
```

To display value of a variable
```
echo $VARNAME
```
<br/>

Create a new global variable. Enclosed the value with double quotes if it contains spaces.
```
export VARIABLE_NAME= variable_value
```
<br/>

Create a new local variable
```
VARIABLE_NAME= variable_value
```
<br/>

Remove a variable
```
unset varname
```
<br/><br/>


### **Package Installation**
```
sudo apt-get install <package_name>
```
<br/>

Or
```
sudo apt install <package_name>
```
<br/><br/>


### **Install .deb Packages**
```
sudo dpkg -i <package_name.deb>
```
<br/><br/>


### **Remove Packages**
```
sudo apt-get remove <package_name>
```
<br/>

Or
```
sudo apt remove <package_name>
```
<br/>

Or
```
sudo apt purge <package_name>
```
<br/>

Remove with force
```
sudo apt-get remove --force-yes <package_name>
```
<br/><br/>


### **Remove .deb Packages**
```
sudo dpkg -r <package_name>
```
<br/>

Or
```
sudo dpkg --purge <package_name>
```
<br/>

Remove with force
```
sudo dpkg -r --force-all <package_name>
```
<br/>

### **Update Packages List**
```
sudo apt-get update
```
<br/>

Or
```
sudo apt update
```
<br/><br/>


### **Upgrade Installed Packages**
```
sudo apt-get upgrade
```
<br/>

Or
```
sudo apt-get dist-upgrade
```
