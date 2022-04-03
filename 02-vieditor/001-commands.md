VI Editing commands
i – Insert at cursor (goes into insert mode)
a – Write after cursor (goes into insert mode)
A – Write at the end of line (goes into insert mode)
ESC – Terminate insert mode
u – Undo last change
U – Undo all changes to the entire line
o – Open a new line (goes into insert mode)
dd – Delete line
3dd – Delete 3 lines.
D – Delete contents of line after the cursor
C – Delete contents of a line after the cursor and insert new text. Press ESC key to end insertion.
dw – Delete word
4dw – Delete 4 words
cw – Change word
x – Delete character at the cursor
r – Replace character
R – Overwrite characters from cursor onward
s – Substitute one character under cursor continue to insert
S – Substitute entire line and begin to insert at the beginning of the line
~ – Change case of individual character


Moving within a file
k – Move cursor up
j – Move cursor down
h – Move cursor left
l – Move cursor right


Saving and Closing the file
Shift+zz – Save the file and quit
:w – Save the file but keep it open
:q – Quit without saving
:wq – Save the file and quit

Change the mode
i - Start typing before the current character
I - Start typing at the start of current line
a - Start typing after the current character
A - Start typing at the end of current line
o - Start typing on a new line after the current line
O - Start typing on a new line before the current line

To jump lines:
Commands    Action
G   Will direct you at the last line of the file
``  Will direct you to your last position in the file
To delete:
Commands    Action
x   Delete the current character
X   Delete the character before the cursor
r   Replace the current character
xp  Switch two characters
dd  Delete the current line
D   Delete the current line from current character to the end of the line
dG  delete from the current line to the end of the file
To repeat and undo:
Commands    Action
u   Undo the last command
.   Repeat the last command
Command to cut, copy and paste:
Commands    Action
dd  Delete a line
yy  (yank yank) copy a line
p   Paste after the current line
P   Paste before the current line
Command to cut, copy and paste in blocks:
Commands    Action
<n>dd   Delete the specified n number of lines
<n>yy   Copy the specified n number of lines
Start and end of line:
Commands    Action
θ   Bring at the start of the current line
^   Bring at the start of the current line
$   Bring at the end ong at end of a line
n   Go to next occurrence of searched string
/\<he\> Search for the word he (and not for there, here, etc.)
/pl[abc]ce  Search for place, plbce, and plcce
Replace all
Syntax:

:<startLine,endLine> s/<oldString>/<newString>/g  
Example:

Commands    Action
:1,$ s/readable/changed/    Replace forward with backward from first line to the last line
:3,6 s/letters/neww/g   Replace forward with backward from third line to the ninth line
Text buffers:
Commands    Action
"add    Delete current line and put text in buffer a
"ap Paste the line from buffer a
Abbreviation
Syntax:

:ab <abbreviation> <abbreviatedWord>  
Example:

Commands    Action
:ab au abbrevition and unabbreviation   Abbreviate au to be 'abbrevition and unabbreviation'
:una au
Un - abbreviate auf the current line
d?  Delete till start of a line
d$  Delete till end of a line
Joining lines:
Commands    Action
J   Join two lines
yyp Repeat the current line
ddp Swap two lines
Move forward or backward:
Commands    Action
w   Move one word forward
b   Move one word backward
<n>w    Move specified number of words forward
dw  Delete one word
yw  Copy one word
<n>dw   Delete specified number of words
Search a string:
Commands    Action
/string Forward search for given string
?string Backward search for given string
/^string    Forward search string at beginning of a line
/string$    Forward search stri

