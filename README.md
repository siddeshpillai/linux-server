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
