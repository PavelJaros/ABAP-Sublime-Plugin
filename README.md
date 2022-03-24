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
 - one more thing - maybe you would like to try out my Marias card game (Czech only) at http://marias.g6.cz/

Recommendation
--------------
I prefer the default color scheme **Zenburnesque** to achieve the best results. 

Go to the main menu: *Preferences -> Color Scheme -> Color Scheme - Default -> Zenburnesque*.

Define own shortcut for ABAP syntax
-----------------------------------
Go to the main menu: *Preferences -> Key Bindings - User*. Place following code inside brackets [ you key bindings here... ]. You can set another shortcut key instead of *ctrl+shift+a*.
<pre><code>
   // Set ABAP synta
   {"keys": ["ctrl+shift+a"], "command": "set_file_type",
    "args": {"syntax": "Packages/ABAP/ABAP.tmLanguage"}
   },
   // shorcut for quick switch project	
   { "keys": ["ctrl+alt+p"], "command": "prompt_select_workspace" },	
</code></pre>
Don't forget to save the file in the end.
