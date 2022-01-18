## Lab 01

- Name:Saraswathi Nagendiran
- Email:nagendiran.2@wright.edu

## Part 1 Answers

1. mkdir DirA
2. mkdir "Dir B"
3. cd "Dir B"
4. DirA is a better naming convention than "Dir B" because spaces should be avoided on the directory / folder name. 
5. mv "Dir B" DirB

## Part 2 Answers

1.vim DirA/test.txt
Press Escape + i
Type 3 lines.. 
Line1
Line2
Line3
Press Escape + :wq 

2. File contents:
cat test.txt
Line1
Line2
Line3


## Part 3 Answers

1. cp test.txt .hiddentest.txt

2.  ls -la DirA
total 16
drwxr-xr-x 2 sarasiva sarasiva 4096 Jan 18 11:35 .
drwxr-xr-x 5 sarasiva sarasiva 4096 Jan 18 11:30 ..
-rw-r--r-- 1 sarasiva sarasiva   19 Jan 18 11:35 .hiddentest.txt
-rw-r--r-- 1 sarasiva sarasiva   19 Jan 18 11:30 test.txt

## Part 4 Answers

1.sudo su - root
adduser bob
exit

2. su bob
 cd
 pwd
 /home/bob
 
3. No another user cannot add files to bob's home directory because there is no permission granted.
touch: cannot touch 'abc.txt': Permission denied

4. su bob

5. cd

6. Yes bob can create files under his home directory because he has permissions.

7. exit

8. cd

## Part 5 Answers

1. addgroup crew
2. usermod -g crew bob
usermod -g crew sarasiva

3. chgrp -R crew DirA
4. su - bob
5. cd /home/sarasiva/DirA
touch bobtest.txt
6. Because bob and sarasiva (my user) are under same group and DirA has group level write access.

## Part 6 Answers

1. sudo touch sudowho.txt
2. -rw-r--r-- 1 root     root    0 Jan 18 17:29 sudowho.txt
3. It is not allowing to save the changes because there is no permission for my user to edit (write) the file as the file is under root access.

## Extra Credit

1. cd DirB
touch mydiary.txt
chmod 600 mydiary.txt

2.chmod 660 mydiary.txt will allow other users in the group to edit the file.
