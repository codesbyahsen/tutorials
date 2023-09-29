# Linux Handbook
Introduction to the linux commands. In this guide, you will learn Linux shell commands and their functionalities.
<br/> <br/>


## Table of Contents
- [What is Linux?](#what-is-linux)
- [Basic Commands](#basic-commands)
- [Environment Variables](#environment-variables)


## **What is Linux?**
<br/><br/>


### **Basic Commands**
Allows regular users to run programs with the security privileges of the superuser or root
```
sudo
```

Command used to install and update packages
```
apt-get
```
Or
```
apt
```

Show all files and directories(folder)
```
ls
```

Show sub-directories as well
```
ls -R
```

Show hidden files as well
```
ls -a
```

Show all files and directories with detail information
```
ls -al
```

Navigate to `Home` directory
```
cd
```
Or
```
cd ~
```

Move one step level up
```
cd ..
```

Move two step level up
```
cd ../..
```

Move to `root` directory
```
cd /
```

Create a new file
```
cat > filename
```

Show the content of the file
```
cat filename
```

Delete file
```
rm filename
```

Gives a list of all past commands typed in the current terminal session
```
history
```

Clears the terminal
```
clear
```

Create new directory
```
mkdir directoryname
```

Delete directory
```
rmdir directoryname
```

To show file type and access permission
```
ls -l
```

(r) - Read
(w) - Write
(x) - Execute
Read, Write, Execute for all
```
chmod 777
```

rwx for owner, rx for group and world
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

Create a new global variable. Enclosed the value with double quotes if it contains spaces.
```
export VARIABLE_NAME= variable_value
```

Create a new local variable
```
VARIABLE_NAME= variable_value
```

Remove a variable
```
unset varname
```
