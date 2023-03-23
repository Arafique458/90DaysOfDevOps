Day 3 Task: Basic Linux Commands

Task: What is the linux command to

1. To view what's written in a file.
2. To change the access permissions of files.
3. To check which commands you have run till now.
4. To remove a directory/ Folder.
5. To create a fruits.txt file and to view the content.
6. Add content in devops.txt (One in each line) - Apple, Mango, Banana, Cherry, Kiwi, Orange, Guava.
7. To Show only top three fruits from the file.
8. To Show only bottom three fruits from the file.
9. To create another file Colors.txt and to view the content.
10. Add content in Colors.txt (One in each line) - Red, Pink, White, Black, Blue, Orange, Purple, Grey.
11. To find the difference between fruits.txt and Colors.txt file.


Reference: https://www.linkedin.com/pulse/linux-commands-devops-used-day-to-day-activit-chetan-/



TASK COMPLETED

devbox@linux-devbox:~/day-3-task$ cat file1.txt 
Day 3 Task: Basic linux Commands
devbox@linux-devbox:~/day-3-task$ git --version
git version 2.34.1
devbox@linux-devbox:~/day-3-task$ chmod 777 file1.txt
devbox@linux-devbox:~/day-3-task$ ls -la
total 12
drwxrwxr-x 2 devbox devbox 4096 Mar 23 00:04 .
drwxr-x--- 6 devbox devbox 4096 Mar 23 00:04 ..
-rwxrwxrwx 1 devbox devbox   33 Mar 23 00:04 file1.txt
devbox@linux-devbox:~/day-3-task$ mkdir testdir
devbox@linux-devbox:~/day-3-task$ touch testfile.txt
devbox@linux-devbox:~/day-3-task$ rmkdir testdir
Command 'rmkdir' not found, did you mean:
  command 'mmkdir' from deb mblaze (1.1-1)
  command 'hmkdir' from deb hfsutils (3.2.6-15build2)
  command 'rmdir' from deb coreutils (8.32-4.1ubuntu1)
  command 'mkdir' from deb coreutils (8.32-4.1ubuntu1)
Try: sudo apt install <deb name>
devbox@linux-devbox:~/day-3-task$ rmdir testdir
devbox@linux-devbox:~/day-3-task$ rm testfile.txt 
devbox@linux-devbox:~/day-3-task$ touch fruits.txt
devbox@linux-devbox:~/day-3-task$ vim fruits.txt
devbox@linux-devbox:~/day-3-task$ vim fruits.txt
devbox@linux-devbox:~/day-3-task$ head -3 fruits.txt 
Apple
Mango
Banana
devbox@linux-devbox:~/day-3-task$ tail -3 fruits.txt 
Kiwi
Orange
Guava
devbox@linux-devbox:~/day-3-task$ touch colors.txt
devbox@linux-devbox:~/day-3-task$ vim colors.txt 
devbox@linux-devbox:~/day-3-task$ diff fruits.txt colors.txt 
1,5c1,5
< Apple
< Mango
< Banana
< Cherry
< Kiwi
---
> Red
> Pink
> White
> Black
> Blue
7c7,8
< Guava
---
> Purple
> Grey
