Make sure to use biber to compile bibliography.

To generate glossaries
1. makeglossaries.exe requires perl interpreter. Make sure to install it. Download here: http://www.activestate.com/activeperl/downloads. DONT forget to add perl to system environment path 
2. run makeglossaries.exe dms.tex in a command line

Additional notes when compiling through TeXStudio IDE
------------------------------------------------------------------
Setting up biber
1. Goto TexStudio: Options -> Configure TeXStudio -> Build -> Meta Commands
2. Inside "Default Bibliography tool" type txs:///biber

Creating custom command for generating glossaries
1. Goto TexStudio: Options -> Configure TeXStudio -> Build -> User Commands
2. Click plus sign
3. Name the command on the left field. On the field input makeglossaries.exe %
   If you want to compile and view glossaries use makeglossaries.exe % | txs:///view