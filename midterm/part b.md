# ANSWER

Create tree in one command 

mkdir -p ~/slg/tutorial3/practice/commands/{command1.txt,command2.txt,command3.txt,command4.txt,command5.txt} ~/slg/tutorial3/practice/examples/{example1.txt,example2.txt,example3.txt,example4.txt,example5.txt,example6.txt} ~/slg/tutorial3/notes/lesson1/{lesson1.txt,lesson1_old.txt} ~/slg/tutorial3/notes/lesson2/{lesson2.txt,lesson2_old.txt}


# Answers to File Operations

```bash
cp ~/slg/tutorial3/practice/commands/command1.txt ~/slg/tutorial3/practice/examples/
```
```bash
cp ../../notes/lesson1/lesson1.txt ../../notes/lesson2/
```
```bash
cp ~/slg/tutorial3/practice/commands/example1.txt ~/slg/tutorial3/practice/examples/
```
```bash
cp ~/slg/tutorial3/notes/lesson2/lesson2.txt ~/slg/tutorial3/practice/commands/
```
```bash
cp ../../practice/commands/example2.txt ../../practice/examples/
```
```bash
mv ~/slg/tutorial3/practice/examples/command2.txt ~/slg/tutorial3/practice/commands/
```
```bash
mv ../../notes/lesson1/lesson1.txt ../../practice/examples/
```
```bash
mv ~/slg/tutorial3/practice/examples/example3.txt ~/slg/tutorial3/notes/lesson1/
```
```bash
mv ~/slg/tutorial3/practice/commands/example4.txt ~/slg/tutorial3/notes/lesson2/
```
```bash
mv ../../notes/lesson2/lesson2.txt ../../practice/examples/
```
```bash
rm ~/slg/tutorial3/practice/commands/command3.txt
```
```bash
rm ../../notes/lesson1/lesson1_old.txt
```
```bash
rm ~/slg/tutorial3/practice/examples/example5.txt
```
```bash
rm ../../practice/commands/command4.txt
```
```bash
rm ~/slg/tutorial3/notes/lesson2/lesson2_old.txt
```
```bash
mv ~/slg/tutorial3/practice/commands/command5.txt ~/slg/tutorial3/practice/commands/
```
```bash
command5_renamed.txt
```
```bash
mv ~/slg/tutorial3/practice/examples/example6.txt ~/slg/tutorial3/practice/examples/
```
```bash
example6_renamed.txt
```
```bash
mv ../../notes/lesson1/lesson1.txt ../../notes/lesson1/lesson1_final.txt
```
```bash
mv ~/slg/tutorial3/notes/lesson2/lesson2.txt ~/slg/tutorial3/notes/lesson2/lesson2_final.txt
```
```bash
mv ~/slg/tutorial3/practice/examples/example1.txt ~/slg/tutorial3/practice/examples/
```
```bash
example1_renamed.txt
```

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
Copy code
ln -s ~/slg/tutorial3/practice/commands/command1.txt ~/slg/tutorial3/practice/commands/soft_link_to_command1.txt
```
```bash
Copy code
ln ~/slg/tutorial3/practice/examples/example1.txt ~/slg/tutorial3/practice/examples/hard_link_to_example1.txt
```
```bash
Copy code
ls -i ~/slg/tutorial3/practice/commands/command1.txt
```
```bash
Copy code
ls -i ../commands/soft_link_to_command1.txt
```
```bash
Copy code
ls -i ~/slg/tutorial3/practice/examples/hard_link_to_example1.txt
```
