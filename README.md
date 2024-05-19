<h1>Manage files with Linux commands</h1>


<h2>Description</h2>
Use Linux commands to modify a directory structure and the files it contains and also use the nano text editor to add text to a file.


<h2>Environments Used </h2>

- <b>Linux</b>
- <b>Bash Shell</b>
- <b>Nano Editor</b>

<h2>Scenario:</h2>

In this scenario, you need to ensure that the /home/analyst directory is properly organized.

You have to make a few changes to the /home/analyst directory and the files it contains.

You also have to edit a file to record the changes or updates you make to the directory.

When you start, the /home/analyst directory contains the following subdirectories and files:
<img src="https://i.imgur.com/ZQoP48q.png" height="80%" width="80%"/>

You need to modify the /home/analyst directory to the following directory and file structure:
<img src="https://i.imgur.com/FIiE5OM.png" height="80%" width="80%"/>

Here’s how you’ll do this: 

<b>First</b>, you’ll create a new subdirectory called logs in the /home/analyst directory. 

<b>Next</b>, you’ll remove the temp subdirectory. 

<b>Then</b>, you’ll move the Q3patches.txt file to the reports subdirectory and delete the tempnotes.txt file. 

<b>Finally</b>, you’ll create a new .txt file called tasks in the notes subdirectory and add a note to the file describing the tasks you've performed.


<h2>Tutorial walk-through:</h2>

<h3>Task 1. Create a new directory</h3>

First, you must create a dedicated subdirectory called logs, which will be used to store all future log files.

1. Create a new subdirectory called logs in the /home/analyst directory.  
2. List the contents of the /home/analyst directory to confirm that you’ve successfully created the new logs subdirectory.

The output should list the original three directories and the new logs subdirectory:

<img src="https://i.imgur.com/5tJQEgP.png" height="80%" width="80%"/>

<h3>Task 2. Remove a directory</h3>

Next, you must remove the temp directory, as you’ll no longer be placing items in it.

1. Remove the /home/analyst/temp directory.
2. List the contents of the /home/analyst directory to confirm that you have removed the temp subdirectory.

The temp directory should no longer be listed:

<img src="https://i.imgur.com/ZzjTsmn.png" height="80%" width="80%"/>

<h3>Task 3. Move a file</h3>

The Q3patches.txt file contains notes taken on third-quarter patches and is now in the correct reporting format.

You must move the  Q3patches.txt file from the notes directory to the reports directory.

1. Navigate to the /home/analyst/notes directory.
2. Move the Q3patches.txt file from the /home/analyst/notes directory to the /home/analyst/reports directory.
3. List the contents of the /home/analyst/reports directory to confirm that you have moved the file successfully.

When you list the contents of the reports directory, it should show that three quarterly report files are now in the reports directory:

<img src="https://i.imgur.com/dAEdEqI.png" height="80%" width="80%"/>

<h3>Task 4. Remove a file</h3>

Next, you must delete an unused file called tempnotes.txt from the /home/analyst/notes directory.

1. Remove the tempnotes.txt file from the /home/analyst/notes directory.
2. List the contents of the /home/analyst/notes directory to confirm that you’ve removed the file successfully.

No files should be listed in the notes directory.

<img src="https://i.imgur.com/J1zEG7F.png" height="80%" width="80%"/>

<h3>Task 5. Create a new file</h3>

Now, you must create a file named tasks.txt in the /home/analyst/notes directory that you’ll use to document completed tasks.

1. Use the touch command to create an empty file called tasks.txt in the /home/analyst/notes directory.
2. List the contents of the /home/analyst/notes directory to confirm that you have created a new file.
   
A file called tasks.txt should now exist in the notes directory:

<img src="https://i.imgur.com/h66TcZl.png" height="80%" width="80%"/>

<h3>Task 6. Edit a file</h3>

Finally, you must use the nano text editor to edit the tasks.txt file and add a note describing the tasks you’ve completed.

1. Using the nano text editor, open the tasks.txt file that is located in the /home/analyst/notes directory.
   <img src="https://i.imgur.com/0jhKenk.png" height="80%" width="80%"/>
2. Copy and paste the following text into the text input area of the nano editor:
   <img src="https://i.imgur.com/S4sC1Gy.png" height="80%" width="80%"/>
3. Press <b>CTRL+X</b> to exit the nano text editor.

This triggers a prompt asking <b>Save modified bufferer?</b>

4. Press <b>Y</b> to confirm that you want to save the new data to your file. (Answering "no" will <b>discard</b> changes.)

5. Press <b>ENTER</b> to confirm that <b>File Name to Write</b> is tasks.txt.
   <img src="https://i.imgur.com/3gRUFrl.png" height="80%" width="80%"/>

6. Use the clear command to clear the Bash shell window and remove any traces of the nano text input area.
   <img src="https://i.imgur.com/BC0kqGy.png" height="80%" width="80%"/>

7. Display the contents of the tasks.txt file to confirm that it contains the updated task details.
   
This file should now contain the contents of the tasks.txt file that you added and saved in previous steps:

<img src="https://i.imgur.com/wHDbzG9.png" height="80%" width="80%"/>



<h2>Conclusion</h2>

You now have practical experience in using basic Linux Bash shell commands to:

- create and remove directories
- copy, move, and remove files
- edit files with the nano text editor

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
