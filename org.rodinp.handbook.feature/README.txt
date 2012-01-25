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


-------------------------------------------------------------------
Linux Installation

  Plastex is available in modern repositories, but it has a horrible
  performance and creates a lot of zombies (but works).
  
  This problem is due to an old version of dvipng.  To solve this, 
  install dvipng 1.14 or better.
  
  Download the .deb from
  http://packages.debian.org/search?keywords=dvipng
  Note: You may have to de-install plastex first, isntall dvipng,
  and then reinstall plastex.
-------------------------------------------------------------------

HOW TO BUILD AN UPDATE SITE
===========================

1. Import the org.rodinp.handbook plugin as an existing eclipse 
project into your eclipse workspace (as a reference) from /build/eclipse.
If you already imported the project you have to refresh the plugin
after building the update site project. 

2.  Goto the org.rodinp.handbook.updatesite plugin and open the
site.xml file.

3. Click on the "Build all" button in order to build the update site.

4. Deploy the files ... i.e. http://handbook.event-b.org/updatesite

CONTACT
=======
Michael Jastram (michael@jastram.de)

