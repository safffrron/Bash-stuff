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
  rm folder_name/s
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

---














