# linux-server

Required Software
If you've already downloaded and installed these items, perhaps while completing a different course, you do not need to download and install these items again.

Download and install VirtualBox. This is free software that will run the virtual machine.
Download and install Vagrant. This is an command line utility that makes it easy to manage and access your virtual machines.

Note: Currently (July 2018), the version of VirtualBox you will want is 5.2. Newer versions do not yet support Vagrant.

Follow these steps to setup an environment where you can work on this course:

1. Create a new folder on your computer where you’ll store your work for this course, then open that folder within your terminal.
2. Type vagrant init ubuntu/trusty64 to tell Vagrant what kind of Linux virtual machine you would like to run.
3. Type vagrant up to download and start running the virtual machine

Commands:
1. ```vagrant status```
This command will show you the current status of the virtual machine. It should currently read “default running (virtualbox)” along with some other information.
2. ```vagrant suspend```
This command suspends your virtual machine. All of your work is saved and the machine is put into a “sleep mode” of sorts. The machines state is saved and it’s very quick to stop and start your work. You should use this command if you plan to just take a short break from your work but don’t want to leave the virtual machine running.
3. ```vagrant up```
This gets your virtual machine up and running again. Notice we didn’t have to redownload the virtual machine image, since it’s already been downloaded.
4. ```vagrant ssh```
This command will actually connect to and log you into your virtual machine. Once done you will see a few lines of text showing various performance statistics of the virtual machine along with a new command line prompt that reads vagrant@vagrant-ubuntu-trusty-64:~$
5. ```vagrant halt```
This command halts your virtual machine. All of your work is saved and the machine is turned off - think of this as “turning the power off”. It’s much slower to stop and start your virtual machine using this command, but it does free up all of your RAM once the machine has been stopped. You should use this command if you plan to take an extended break from your work, like when you are done for the day. The command vagrant up will turn your machine back on and you can continue your work.
6. ```vagrant destroy```
This command destroys your virtual machine. Your work is not saved, the machine is turned off and forgotten about for the most part. Think of this as formatting the hard drive of a computer. You can always use vagrant up to relaunch the machine but you’ll be left with the baseline Linux installation from the beginning of this course. You should not have to use this command at any time during this course unless, at some point in time, you perform a task on the virtual machine that makes it completely inoperable.

## Some handy stuffs
1. ```sudo apt-get update``` Updates the package list
2. ```sudo apt-get upgrade``` Updates the packages
3. ```sudo apt-get install finger``` Instals the package named finger
4. ```finger``` gets the user information of all the users
5. ```finger <user>``` gets the information about the user
6. ```cat /etc/passwd``` It actually reads the information from /etc/passwd to get the information
7. ```sudo addusr <user>``` to add a new user 
8. ```sudo finger <user>``` to confirm whether the user was created

Now, open a new terminal to connect to the user that we created above

9. ```ssh <user>@127.0.0.1 -p 2222``` remember in the above steps we did ```vagrant ssh``` which is a shorthand command for vagrant user. 127.0.0.1 is the local host 2222 is the port no that you want to establish the connection
