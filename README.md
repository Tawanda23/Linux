# Linux

This is a walk through of how to install Virtualbox, create a virtual machine and everyday Linux commands.

## Virtualbox Install & Vagrant Set-up

Virtualbox is required to be able to ins

Vagrant is designed to run on the local machine to create a Viryual MAchine inside.

To install, follow these steps:

Ensure there is enough memory on the local machine that the virtual machine will be created on.

1. Go to [VirtualBox Downloads](https://www.virtualbox.org/wiki/Downloads)
    - The latest version of virtualbox will need to be installed

2. Follow installation instructions

Before creating a virtual machine, Vagrant needs to be installed and configured.

To set up Vagrant, follow these steps:

1. Create a folder where you want to store the virtual machine files.
2. Navigate to the newly created folder in your terminal.
3. Search for the desired box on the Vagrant website, e.g., `ubuntu/jammy64`.
4. Initialize the Vagrant configuration file by running: `vagrant init ubuntu/jammy64`
![present working directory](/images/vagrant-init.png)

5. `vagrant init ubuntu/jammy64` - this will create the vagrant file that will be used to configure an Ubuntu machine

6. `vagrant up` - This will start the virtual machine

7. `vagrant-ssh` - SSH in to the machine

`sudo apt-get update -y` - thsi comamand will auto-updte all the updates required when the virtual machine is started

`sudo su` - changes to root user

## Naviagating Command Line

`pwd` - shows the current working directory
![present working directory](/images/pwd.png)

`ls` - Lists the contents of the current directory

`cd` - changes directory

`whoami` - command will show which user is currently logged in

`clear` - clears the terminal


##  Creating Files and Directories

 `mkdir` - this command creates a folder in the designated working directory. This is command expects a follow up command

![present working directory](/images/mkdir.png)

`touch` - this command will create a file in the folder selected
    ![present working directory][def]

 `cat` - looks at the contents of the file 
![present working directory](/images/cat.png)

To save changes made in a file, press `Ctrl + X`, then `Y`, and finally `Enter`.

To delete files and directories:

- `rm <file_name>`: Deletes a file.
- `rmdir <directory_name>`: Deletes an empty directory.

Files and directories can be moved around directories using the 'mv' command:

`mv <filename> <directory destinantion>`
![present working directory](/images/mv.png)

To install further packages in Linux, user needs to be Root User to have the necessary permission.
