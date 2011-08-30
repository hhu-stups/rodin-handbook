OVERVIEW
========

This project holds the Rodin Handbook and the scripts to publish it.

This feature has two purposes:

1. A container for the content and scripts for the Rodin Handbook

2. A feature that includes the documentation into Eclipse.

HOW TO BUILD
============
1. Install Plastex on your system (http://plastex.sourceforge.net/)

-------------------------------------------------------------------
Windows Installation: 
	1. Follow the instructions in INSTALL
	2. Create a plastex.bat with the following content 
		"C:\Python27\python.exe C:\Python27\Scripts\plastex %1"
		Please note that you have to adapt the Python installation path!
	3. Add the path to the plastex.bat to your windows environment path
-------------------------------------------------------------------	
2. Install Rubber on your system (https://launchpad.net/rubber)
3. Run the build.xml ant file

The resulting HTML and Eclipse Plugin with Eclipse help will be in the build folder.

HOW TO BUILD AN UPDATE SITE
============

1. Import the org.rodinp.handbook plugin (included in the /build/plugin/org.rodinp.handbook.zip)
as an existing eclipse project into your eclipse workspace.
2.  Right click on the org.rodinp.feature 
--> Export --> Plug-in Development --> Deployable features
3. Please be sure that you have checked "Generate metadata repositiory" and 
selected the category.xml in "Categorize repository" in the "Options" tab.
4. Deploy the files ... i.e. http://handbook.event-b.org/updatesite

CONTACT
=======
Michael Jastram (michael@jastram.de)

