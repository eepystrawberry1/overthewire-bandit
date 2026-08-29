#level 0:
**Commands used:** "ssh" (allows to operate network services remotely).
**Syntax:** "ssh username@hostname -p portnb"
#level0--> level1:
**commands used** "cat" (to extract what's inside for the file) "exit" (needed so u can use ssh to log into the next level) 
#level1-->level2:
**what i learned** Can't use the command "cat" on a file named - you have to add ./ or .. before the -
#level2-->level3:
**what i learned** for when a file name has spaces you add -- before file name (and file name between "") 
#level3-->level4:
**commands used** "cd" (moves u to the directory u name), "ls -la" (lists in details the content of the whole directory including the hidden files), "cat+." (we add the . when the file is hidden). 
level4-->level5:
**commands used** "file" (tells u what type of data ur file is in), using "*" means including every single file in the directory
[cat works one files]
[cd works on directories] 
#level5-->level6:
**commands i used**: "find" (reaches subdirectories and subdolders 
find . -type f (search inside current directory (.) for a regular file (type f))
level6-->level7:
**commands i used**: "find /" (searches starting from the root), 
["find" output is a file path] 
#level7-->level8:
**what i learned**: "grep" (used to find lines that match pattern you gave) 
#level8-->level9:
**commands i used**: "uniq" only compares line next to eachother so u hv to use "sort" (groups the identical lines together)
**what i learned**: we can use two commands in one line separated by | (the output of the first command is the input of the second command). 
exp: sort data.txt | uniq -u 
