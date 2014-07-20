-----

*Southwest Research Institute*
![alt tag](http://www.boulder.swri.edu/clark/swrilogo.gif)

**Author:** Zach Dischner

**Description:** Doxygen setup for generic project. Work in progress...

**Dependancies:** These dependancies are listed as standard Ubuntu linux package names that can be installed via "apt-get", "pip", or maybe "homebrew":

doxygen python

========= 

## Setup

**NOTE, THIS WILL NOT WORK IF YOUR DIRECTORY FOLDERS HAVE SPACES IN THEIR NAMES.**
**I suspect that is a feature of doxypypy, but instead of `python modules`, directories must be named `python_modules` or something similar**

###As intended, within working git repository
From the top level of project already managed by git, containing appropriately documented C/Python/Java etc code

	git submodule add https://github.com/ZachDischner/DoxyDocs.git doc
	cd doc
	git submodule init
	git submodule update

###Within raw project folder
From the top level of a project not managed by git (ANARCHY!!!!). Perform a recursive clone instead of a submodule addition. 

	git clone --recursive https://github.com/ZachDischner/DoxyDocs.git doc


##Usage
Configure the doc/Doxyfile-Python to point to specific directories, for now it just looks one directory up (doc/..) and recursively searches for appropriate files

	cd doc
	doxygen Doxyfile-Python
	open html/index.html

View code generated documentation in doc/html/index.html

*SOMETIME PUT TOGETHER A REPO EXAMPLE


