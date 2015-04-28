# Introduction #
This is how to build the ITR controller, assuming a fresh Ubuntu install (Commands will also work for debian, and most will work for others, but you'll have to find packages yourself)

(Since I dont know Wiki markup, code snippits to be run in terminal are on their own line, and bolded)


# Setup Build Requirements #

On Ubuntu / Debian, this consists of getting the packages: build-essential libsdl1.2debian-all libsdl1.2-dev

**sudo apt-get install libsdl1.2debian-all libsdl1.2-dev build-essential**

To get the compilation tools for the gumstix / robostix, first download the gbr.tar.bz2 package off the downloads page. After that has downloaded, (assuming it was downloaded to the desktop, change the cd to the downloads directory if not), run:

**cd ~/Desktop && sudo tar -xvjf gbr.tar.bz2 -C /**

This should put you into a build ready state.

# Getting the code #

Follow directions on the Checkout subtab of the Source tab in this project. The location of the code on your computer doesnt matter.

# Building the code #

In terminal, cd to itr-jsdc-controller (Wherever you checked it out to), and type:

**make**

That shouldn't return an error (The last line should be "make[1](1.md): leaving directory ..." and not an error line)

in the controller or robot directories, make <robot name> will make just that robot's controller or robot, respectively.