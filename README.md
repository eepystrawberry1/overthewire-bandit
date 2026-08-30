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
exp: grep+ what u r looking for between '
#level8-->level9:
**commands i used**: "uniq" only compares line next to eachother so u hv to use "sort" (groups the identical lines together)
**what i learned**: we can use two commands in one line separated by | (the output of the first command is the input of the second command). 
exp: sort data.txt | uniq -u 
#level9-->level10:
**commands i used**: "strings" (outputs the text existing within binary data in a file)
#level10-->level11:
**commands i used**: "base64 -d filename" (decodes the file to readable text)
#level11-->level12: 
**commands i used**: "tr" (used when Rot13 is needed)+ has other uses.
#level12-->level13:
**commands i used** "xxd" (make a hexdump or the reverse (xxd -r)), "mktemp" (to create a temporary file or directory) [mktemp -d creates a uniq temporary directory no one can use], "cp" (copies the wanted file into the wanted destination , if not specified its copied into your working directory), "file filename" (tells u what the original type of the content is), "gzip -d" (unpacks a gzip type file, should end in [.gz]), "bzip2 -d" (unpacks a bzip2 type file, should end in [.bz2]), "tar -xf" (unpacks type tar archive data, should end in [.tar])
**what i learned**: /tmp is a standard system directory in Linux OS used to store temporary files. A compressed Linux file changes its original extension.
