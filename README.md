-----

*Southwest Research Institute*
![alt tag](http://www.boulder.swri.edu/clark/swrilogo.gif)

**Author:** Zach Dischner

**Description:** Doxygen setup for generic project. Work in progress...

**Dependancies:** These dependancies are listed as standard Ubuntu linux package names that can be installed via "apt-get", "pip", or maybe "homebrew":

doxygen python

========= 

## Usage
From within working project directory, with appropriately documented python/C/Java code...
	git submodule add https://github.com/ZachDischner/DoxyDocs.git doc

Configure the Doxyfile-Python to point to specific directories, for now it just looks one directory up (doc/..) and recursively searches for appropriate files

	cd doc
	doxygen Doxyfile-Python

View code generated documentation in doc/html/index.html
