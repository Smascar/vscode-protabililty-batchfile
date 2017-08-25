# vscode-protabililty-batchfile
File for making Visual Code Studio store it's dependencies within the same folder itself, very important if you keep your text editor on a pendrive and move around a lot.

Why did i do this?
  I'm a college student and when I work at home,
                                                I use Vs Code/Sublime
                                        in College,
                                                They use **Notepad** (No joke), but i love to use VSC there too.

  Now the best part is that VSC comes in a zip file and can just be put on a pen drive. All sunshine and puppies till I realised that the   extensions have to be downloaded again when i shift to any new pc and settings too don't survive the migration.
  
  So i made this batch file with the intent to tell the program to start with certain parameters like where to store the extension and the   settings/cache files.
	
	I found the syntax on Microsoft's site itself and also where does VSC store the folders.
	
**Store this file in the folder itself**
**To open VSC click on this file and not on the application**

Note: 
In the file, the following code resides:
>**start** code **--extensions-dir** extensions **--user-data-dir** Code

**Bold:** Compulsary.
code -> application name/exe file to open.
extensions -> folder name for the extensions.
Code -> folder name for the cache/settings files.

Now if you want to keep this file elsewhere, you **have** to put the address to that location. 
Example if i want to keep my file outside of my folder which has the name 'vsc', then
>**start** vsc\code **--extensions-dir** vsc\extensions **--user-data-dir** vsc\Code
