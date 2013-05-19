ABAP-Sublime-Plugin
===================

Description: **ABAP Syntax Highlighter for Sublime Text 2**

How to install it?
------------------
 - Open your **Package folder**. The easiest way to identify the Package folder is to go to ST2 main menu: *Preferences -> Browse Packages...* 
 - Manualy create *ABAP* folder under your Package folder: *...\Packages\ABAP*
 - Extract the content of zip archive into the *ABAP* folder (!!only the files without *ABAP-Sublime-Plugin-master* folder!!).

**Location of Package folder according your platform:**
 - Windows Vista/7: *c:\Users\[UserName]\AppData\Roaming\Sublime Text 2\Packages* 
 - OS X/Unix-like: *~/Library/Application Support/Sublime Text 2/Packages*

Important notes
---------------
 - If the file you are editing has *.abp* extension, syntax highlighting works automaticaly. Otherwise you have to set the ABAP syntax explicitely (click on the bottom right corner in the ST2 window a choose ABAP).
 - It's quite simple to add more file extensions by editing **ABAP.tmLanguage** file (located in your ABAP plugin folder under Package folder). Search for *fileTypes* section in the beginning of the file and add for example line *&lt;string&gt;txt&lt;/string&gt;* after the line *&lt;string&gt;abp&lt;/string&gt;*.
 - If nothing works, restart ST2!

What you can do with ABAP plugin
--------------------------------
 - highlight ABAP syntax (keywords, system contstants, name of forms, classes, methods and modules)
 - auto-complete code (it works both keyword suggesting and the snippets)
 - speed up coding with the set of predefined snippets (of course it's very easy to create your owns)
 - get overview of forms, classes, methods and modules on *Ctrl+R* command
 - comment/uncomment selected blocks of code on *Ctrl+/* command
 - for more info please visit my website: http://www.jaros.in/item/abap-syntax-highlighting-for-sublime-text

Recommendation
--------------
I prefer the color scheme **Zenburn** to achieve the best results. 
You can install it either by *Package Control* (press Shift+Ctrl+P -> write *Package Control: Install Package* [Enter] -> write *Zenburn* [Enter]) 
or manualy (download it from https://github.com/colinta/zenburn).
