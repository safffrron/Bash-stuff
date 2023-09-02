## Bash-stuff
<pre>man</pre>
Shows the manual , basically all the commands you can use . 

---
<pre>
  ls
  ls -al
</pre>
If you add a folder name or path, it will print that folder's contents . <br>
-a shows the hidden folders . <br>
-l list files one per line 

---
<pre>cd</pre>
Takes you to that directory .
<br> Short form for change directory .

---
<pre>pwd</pre>
Shows you your current location .

---
<pre>
  mkdir folder_name/s
  mkdir -p folder/nested_folder/s
</pre>
Make folders <br>
-p allows you to make nested folders .

---
<pre>
  rmdir folder_name/s
</pre>
Remove folders <br>
Do not delete non-empty folders 

<pre>
  rm -rf folder_name/s
</pre>
To delete non-empty folders . <br>
Be careful as this command does not ask for confirmation and it will immediately remove anything you ask it to remove.<br>
There is no bin when removing files from the command line, and recovering lost files can be hard.

---
<pre>
  mv folder/s target_folder
</pre>
Moves folders. <br>
If the last parameter is a folder, the file located at the first parameter path is going to be moved into that folder.
<br> In this case, you can specify a list of files and they will all be moved in the folder path identified by the last parameter

---
<pre>
  cp -r folder/s target_folder
</pre>
Copy folders. 
<br> -r to allow it to copy it's content .

---
<pre>
  open file_name 
  open folder_name 
</pre>
Open file / folder. 

<pre>
  open .
  open ..
</pre>
Open . will open the current directory.<br> Open .. will open the parent directory 


---

<pre>
  touch file_name/s 
</pre>
Create a file named file_name in the currrent directory.
<br> If the file already exists, it opens the file in write mode, and the timestamp of the file is updated.

---

<pre>
  find . -name "*.ext"
</pre>
Find all the files under the current tree that have the .ext extension and print the relative path of each file that matches.

<pre>find . -type d -name src</pre>

<br> Find directories under the current tree matching the name "src".<br>
Use -type f to search only files, or -type l to only search symbolic links.
<br><br>
-name is case sensitive. 
<br>Use -iname to perform a case insensitive search.
<br><br>
You can search under multiple root trees:
<pre>find folder1 folder2 -name filename.txt</pre>
Find directories under the current tree matching the name "node_modules" or 'public':

<pre>find . -type d -name node_modules -or -name public </pre>
You can also exclude a path using -not -path:

<pre>find . -type d -name '*.md' -not -path 'node_modules/*'</pre>
You can search files that have more than 100 characters (bytes) in them:

<pre>find . -type f -size +100c</pre>
Search files bigger than 100KB but smaller than 1MB:

<pre>find . -type f -size +100k -size -1M</pre>
Search files edited more than 3 days ago:

<pre>find . -type f -mtime +3</pre>
Search files edited in the last 24 hours:

<pre>find . -type f -mtime -1</pre>
You can delete all the files matching a search by adding the -delete option. This deletes all the files edited in the last 24 hours:

<pre>find . -type f -mtime -1 -delete</pre>
You can execute a command on each result of the search. In this example we run cat to print the file content:

<pre>find . -type f -exec cat {} \;</pre>
Notice the terminating \; <br>{} is filled with the file name at execution time.

---

<pre>
  clear 
</pre>
Clean the terminal.

---

<pre>
  
</pre>




