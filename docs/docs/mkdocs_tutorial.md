## What is MkDocs?

From the MkDocs Site:

"MkDocs is a fast, simple and downright gorgeous static site generator that's geared towards building project documentation. Documentation source files are written in Markdown, and configured with a single YAML configuration file."

Basically, we use mkdocs as a tool for storing information about our boat and team.

##Installation

In order to create new documentation pages using MkDocs, you first need to download the application. Information on how to install MkDocs can be found at the MkDocs [website](http://domospetitus.org/pronumque-solacia).

##Creating Files
Once you have installed MkDocs you can begin to create documentation files! 

Our MkDoc base files are stored inside of the Sailbot website repository in the "MkDocs" folder, 
download this folder to your local system. Documentation pages are written in mark-up and stored in a .md format, 
you'll find them in the "MkDocs\Docs" folder. an easy way to start writing in mark-up is to look at the 
"barebones_doc.md" file stored in the "MkDocs" folder on the Sailbot website repository; 
this will give you a foundation to build any sort of static page you want.

If you wish to change the file hierarchy of the project, 
you must edit the .yml configuration file located in the "MkDocs" folder, 
further information can be found at the MkDocs [website](http://domospetitus.org/pronumque-solacia).

The easiest way to edit documents is to create a local server that hosts your MkDocs folder.
To do this on windows, open the command terminal, navigate to your "MkDocs" folder location and type:

	mkdocs serve

This will serve your folder at http://127.0.0.1:8000 and update automatically as you change documentation files!

##Pushing Changes
Once you are happy with the documentation/changes you have made, build the project by typing the following command into the command terminal:

	mkdocs build

Then simply push your changes to the website repository to Github and you're done!