# beginner_tutorials

## Overview

This is my journey to learn ROS. I started with ROS Melodic so first you need to install the ROS distro (ROS version like Indigo, Kinetic, Melodic etc.). Following is the link to install ROS Melodic:

http://wiki.ros.org/melodic/Installation/Ubuntu

I will suggest that you go with Desktop-Full Install. This way you don't need to be worried about few packages that you'll need in the beginning.

But if you already have some experience and know what you are doing be my guest and jump right into whatever you are looking.


## Dependencies

The following dependencies are required to install ROS Melodic:

- Ubuntu 18.04

Here is a link to a website. There are several other websites and blogs but I just liked how this one guides step-by-step through the installation. 
 
https://www.linuxtechi.com/ubuntu-18-04-lts-desktop-installation-guide-screenshots/ 

NOTE: This should be your first step before you go and try to install ROS Melodic.

Now that you have Ubunutu 18.04 and ROS Melodic running, go and make sure you have catkin tools.

No need to worry. Just go to this link and run the commands to install the catkin_tools:

https://catkin-tools.readthedocs.io/en/latest/installing.html

NOTE: Simply installing it with pip should be enough. But if you still run into problem try with apt-get.

## Get started

Now let's create a catkin workspace.

Just think of 'catkin workspace' as your working place where you work with programs and files that are to be run using ROS. 

In usual case, when you write any program (C++ programs to be specific) how do you compile it ?

1. You write your code in any text editor (like VS Code, SUblime, Atom anything that you use) or an IDE and save your code with a filename and add an extension at the end of that name- '.cpp'

2. Now you open a terminal or bring the terminal from your the menu (in case of IDE like VS Code). 

3. Navigate to the folder where the file has been saved.

4. Once you are in the folder, you type 'g++ filename.cpp'

5. Nothing happened, right ? Kidding!!! A new file is created with the name format like this: 'a.out'

6. This is an executable file. Now you type: ./a.out 

7. And voila! Your program ran!

8. Just imagine doing this for at least 10 different code files (if not hundred) individually.

9. That's where catkin tools come in. These tools are used to compile all the code files in your workspace and create their executable versions ready without your help.

10. That's why you need to have catkin workspace to work with ROS. But how do we get one ? Run following commands in your terminal (in /home directory) to have a catkin workspace.

mkdir -p ~/catkin_ws/src

NOTE: You can have any name as your workspace but it is good to have 'ws' after your worskpace name so that you can identify it easily among your other folders present there (trust me it helps!).

cd ~/catkin_ws/

NOTE: 'cd' means change directory and this command takes you to the workspace directory that you just created in your home directory.

catkin_make

NOTE: When this command runs successfully, Congratulate yourself! You have created a catkin workspace.