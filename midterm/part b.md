# ANSWER

# Create Directory Structure and Files in One Command

The following command creates a directory structure and specific files in a single line:

```bash
mkdir -p ~/slg/tutorial3/{practice/{commands,examples},notes/{lesson1,lesson2}}
&&
touch ~/slg/tutorial3/practice/commands/command{1..5}.txt
~/slg/tutorial3/practice/examples/example{1..6}.txt
~/slg/tutorial3/notes/lesson1/{lesson1.txt,lesson1_old.txt}
~/slg/tutorial3/notes/lesson2/{lesson2.txt,lesson2_old.txt}
```
Explanation
mkdir -p:

mkdir: This command is used to create directories.
-p: This option tells mkdir to create parent directories as needed, without throwing an error if the directory already exists.
Directory Structure:

~/slg/tutorial3/{practice/{commands,examples},notes/{lesson1,lesson2}}:
This part creates the following directories:
practice
commands
examples
notes
lesson1
lesson2
&&:

This operator allows the second command to execute only if the first command (mkdir) is successful.
Creating Files:

touch: This command creates empty files or updates the timestamps of existing files.
File Creation:
~/slg/tutorial3/practice/commands/command{1..5}.txt: This uses brace expansion to create five files:
command1.txt
command2.txt
command3.txt
command4.txt
command5.txt
~/slg/tutorial3/practice/examples/example{1..6}.txt: This similarly creates six files:
example1.txt
example2.txt
example3.txt
example4.txt
example5.txt
example6.txt
~/slg/tutorial3/notes/lesson1/{lesson1.txt,lesson1_old.txt}: This creates two files:
lesson1.txt
lesson1_old.txt
~/slg/tutorial3/notes/lesson2/{lesson2.txt,lesson2_old.txt}: This creates two files:
lesson2.txt
lesson2_old.txt



# Answers to File Operations

<br>
<br>

## For absolute path please replace **colokpedje** which is my username with your own username

<br>
<br>
Copying Files
Copy command1.txt from the commands directory to the examples directory using an absolute path:

```bash

cp /home/colokpedje/slg/tutorial3/practice/commands/command1.txt /home/colokpedje/slg/tutorial3/practice/examples/
```
Explanation: This command copies command1.txt from the commands directory to the examples directory using its full path.
Copy lesson1.txt from the notes/lesson1 directory to the notes/lesson2 directory using a relative path:

```bash

cp ../notes/lesson1/lesson1.txt ../lesson2/
```
Explanation: This command copies lesson1.txt from the lesson1 directory to the lesson2 directory, using a relative path that goes up one level.
Copy example1.txt from the commands directory to the examples directory using an absolute path:

```bash

cp /home/colokpedje/slg/tutorial3/practice/commands/example1.txt /home/colokpedje/slg/tutorial3/practice/examples/
```
Explanation: This copies example1.txt from the commands directory to the examples directory using its full path.
Copy lesson2.txt from the notes/lesson2 directory to the commands directory using a home path:

```bash

cp /home/colokpedje/slg/tutorial3/notes/lesson2/lesson2.txt /home/colokpedje/slg/tutorial3/practice/commands/
```
Explanation: This command copies lesson2.txt from the lesson2 directory to the commands directory, specifying the full path.
Copy example2.txt from the commands directory to the examples directory using a relative path:

```bash

cp ../commands/example2.txt ../examples/
```
Explanation: This copies example2.txt from the commands directory to the examples directory using a relative path.
Moving Files
Move command2.txt from the examples directory to the commands directory using an absolute path:

```bash

mv /home/colokpedje/slg/tutorial3/practice/examples/command2.txt /home/colokpedje/slg/tutorial3/practice/commands/
```
Explanation: This command moves command2.txt from the examples directory to the commands directory using its full path.
Move lesson1.txt from the notes/lesson1 directory to the examples directory using a relative path:

```bash

mv ../notes/lesson1/lesson1.txt ../examples/
```
Explanation: This moves lesson1.txt from the lesson1 directory to the examples directory using a relative path.
Move example3.txt from the examples directory to the lesson1 directory using an absolute path:

```bash

mv /home/colokpedje/slg/tutorial3/practice/examples/example3.txt /home/colokpedje/slg/tutorial3/notes/lesson1/
```
Explanation: This moves example3.txt from the examples directory to the lesson1 directory using its full path.
Move example4.txt from the commands directory to the notes/lesson2 directory using a home path:

```bash

mv /home/colokpedje/slg/tutorial3/practice/commands/example4.txt /home/colokpedje/slg/tutorial3/notes/lesson2/
```
Explanation: This command moves example4.txt from the commands directory to the lesson2 directory.
Move lesson2.txt from notes/lesson2 to examples using a relative path:

```bash

mv ../notes/lesson2/lesson2.txt ../examples/
```
Explanation: This moves lesson2.txt from the lesson2 directory to the examples directory using a relative path.
Removing Files
Remove command3.txt from the commands directory using an absolute path:

```bash

rm /home/colokpedje/slg/tutorial3/practice/commands/command3.txt
```
Explanation: This command removes command3.txt from the commands directory using its full path.
Remove lesson1_old.txt from the notes/lesson1 directory using a relative path:

```bash

rm ../notes/lesson1/lesson1_old.txt
```
Explanation: This removes lesson1_old.txt from the lesson1 directory using a relative path.
Remove example5.txt from the examples directory using a home path:

```bash

rm /home/colokpedje/slg/tutorial3/practice/examples/example5.txt
```
Explanation: This command removes example5.txt from the examples directory using its full path.
Remove command4.txt from the commands directory using a relative path:

```bash

rm ../commands/command4.txt
```
Explanation: This removes command4.txt from the commands directory using a relative path.
Remove lesson2_old.txt from the notes/lesson2 directory using an absolute path:

```bash

rm /home/colokpedje/slg/tutorial3/notes/lesson2/lesson2_old.txt
```
Explanation: This command removes lesson2_old.txt from the lesson2 directory using its full path.
Renaming Files
Rename command5.txt in the commands directory to command5_renamed.txt using a relative path:

```bash

mv ../commands/command5.txt ../commands/command5_renamed.txt
```
Explanation: This renames command5.txt to command5_renamed.txt in the commands directory using a relative path.
Rename example6.txt in the examples directory to example6_renamed.txt using an absolute path:

```bash

mv /home/colokpedje/slg/tutorial3/practice/examples/example6.txt /home/colokpedje/slg/tutorial3/practice/examples/example6_renamed.txt
```
Explanation: This renames example6.txt to example6_renamed.txt in the examples directory using its full path.
Rename lesson1.txt in the lesson1 directory to lesson1_final.txt using a relative path:

```bash

mv lesson1/lesson1.txt lesson1/lesson1_final.txt
```
Explanation: This renames lesson1.txt to lesson1_final.txt in the lesson1 directory using a relative path.

## Hints

1. *(Source Path: `~/slg/tutorial3/practice/commands/command1.txt`, Target Path: `~/slg/tutorial3/practice/examples/command1.txt`)*


2. *(Source Path: `~/slg/tutorial3/notes/lesson1/lesson1.txt`, Target Path: `~/slg/tutorial3/notes/lesson2/lesson1.txt`)*

3. *(Source Path: `~/slg/tutorial3/practice/commands/example1.txt`, Target Path: `~/slg/tutorial3/practice/examples/example1.txt`)*

4. *(Source Path: `~/slg/tutorial3/notes/lesson2/lesson2.txt`, Target Path: `~/slg/tutorial3/practice/commands/lesson2.txt`)*

5. *(Source Path: `~/slg/tutorial3/practice/commands/example2.txt`, Target Path: `~/slg/tutorial3/practice/examples/example2.txt`)*

6. *(Source Path: `~/slg/tutorial3/practice/examples/command2.txt`, Target Path: `~/slg/tutorial3/practice/commands/command2.txt`)*

7.  *(Source Path: `~/slg/tutorial3/notes/lesson1/lesson1.txt`, Target Path: `~/slg/tutorial3/practice/examples/lesson1.txt`)*

8. *(Source Path: `~/slg/tutorial3/practice/examples/example3.txt`, Target Path: `~/slg/tutorial3/notes/lesson1/example3.txt`)*

9. *(Source Path: `~/slg/tutorial3/practice/commands/example4.txt`, Target Path: `~/slg/tutorial3/notes/lesson2/example4.txt`)*

10. *(Source Path: `~/slg/tutorial3/notes/lesson2/lesson2.txt`, Target Path: `~/slg/tutorial3/practice/examples/lesson2.txt`)*

11. *(Path: `~/slg/tutorial3/practice/commands/command3.txt`)*

12. *(Path: `~/slg/tutorial3/notes/lesson1/lesson1_old.txt`)*

13.  *(Path: `~/slg/tutorial3/practice/examples/example5.txt`)*

14. *(Path: `~/slg/tutorial3/practice/commands/command4.txt`)*

15. *(Path: `~/slg/tutorial3/notes/lesson2/lesson2_old.txt`)*

16.  *(Old Path: `~/slg/tutorial3/practice/commands/command5.txt`, New Path: `~/slg/tutorial3/practice/commands/command5_renamed.txt`)*

17. *(Old Path: `~/slg/tutorial3/practice/examples/example6.txt`, New Path: `~/slg/tutorial3/practice/examples/example6_renamed.txt`)*

18.  *(Old Path: `~/slg/tutorial3/notes/lesson1/lesson1.txt`, New Path: `~/slg/tutorial3/notes/lesson1/lesson1_final.txt`)*

## Section 2


```bash
   touch ~/slg/tutorial3/practice/commands/new_file.txt
   ```

```bash
touch ../examples/temp_file.txt
```

```bash

ln -s ~/slg/tutorial3/practice/commands/command1.txt ~/slg/tutorial3/practice/commands/soft_link_to_command1.txt
```
```bash

ln ~/slg/tutorial3/practice/examples/example1.txt ~/slg/tutorial3/practice/examples/hard_link_to_example1.txt
```
```bash

ls -i ~/slg/tutorial3/practice/commands/command1.txt
```
```bash

ls -i ../commands/soft_link_to_command1.txt
```
```bash

ls -i ~/slg/tutorial3/practice/examples/hard_link_to_example1.txt
```
