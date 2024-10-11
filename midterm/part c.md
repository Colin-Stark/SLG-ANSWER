```
How many binary digits does 1 octal digit represent?
1 octal digit represents 3 binary digits.

Manual Numbering Conversion Table:

Octal	Binary
640	1101000000
145	001100101
755	111101101
chmod Command for Pass-Through Permissions (Symbolic Method):
To set "pass-through" permissions (rwx--x--x) for your home directory using an absolute pathname:


chmod u=rwx,g=x,o=x /home/your_username/
Verify Permissions:
To verify that permissions were set:


ls -ld /home/your_username/
Binary to Octal Conversion for Permissions:
The permissions rwx--x--x in binary are:

rwx = 111 (7)
--x = 001 (1)
--x = 001 (1)
So, the octal representation is 711.
Set Pass-Through Permissions Using Absolute Method (Octal Numbers):


chmod 711 /home/your_username/
Add Read Permissions for Group Members:
To add read permissions for the same group members for the ~/tests directory:


chmod g+r ~/tests
Remove Write Permissions for Same Group Members and Others:
To remove write permissions for the same group members and other group members for the ~/projects directory:


chmod go-w ~/projects
Set Permissions for the ~/assignments Directory:
To set the permissions for the ~/assignments directory to rwxr-x--x using the absolute method (octal numbers):

Binary Representation:
User (Owner): rwx = 111 (7)
Group: r-x = 101 (5)
Others: --x = 001 (1)
The octal representation is 751.
The command is:

chmod 751 ~/assignments
Using Octal Numbers with a Relative-to-Home Pathname:
If you just issued:


chmod u=rwx,go=x ~/linux/content
The new permissions for the "content" directory would be:

User: rwx (7)
Group: --x (1)
Other: --x (1)
In octal, this is 711.
Permissions for Newly Created Directory and File:
After issuing:


umask 077
mkdir mydir
touch mydir/myfile.txt
The permissions will be:

mydir: drwx------ (700)
myfile.txt: -rw------- (600)
Bash Shell Script Code:


#!/bin/bash
clear
echo "Hello World"
Permissions Required to Run the Bash Shell Script:
The permissions required to run this script are execute (x) permission for the user:


chmod u+x script.sh
Different Methods to Run the Bash Shell Script:

Using ./ if it’s in the current directory:

./script.sh
Using bash command:

bash script.sh
Using sh command:

sh script.sh
Bash Shell Script for User Interaction:


#!/bin/bash
clear
echo "Please enter your full name:"
read full_name

echo "Please enter your age:"
read age
clear
echo "Welcome, $full_name! You are $age years old."
```
