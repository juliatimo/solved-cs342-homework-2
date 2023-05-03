Download Link: https://assignmentchef.com/product/solved-cs342-homework-2
<br>
Q1. Write a C program in Linux that will create 2^k processes (k &lt;=5), including the initial main program, and will print their pids (process identifiers). The processes will form a complete binary tree.  You will use fork(). The order of printing IDs is not important. You can learn the pid of a process with getpid() system call. The pid of a child created with fork() is returned as the return value of the fork().

Q2. Find out the task_struct structure definition in Linux kernel source code and write the names of 10 fields in that structure.

Q3. How many processes are created by the following pseudo-code:

for (i = 0; i &lt; 5; ++i) {

n = fork();

if (n == 0)  {                if (i % 2 == 0) {

exit(0);

}

}

}




Q4. Which integers are printed out by the following program pseudo-code (order is not important)?




main () { int x = 100;  if fork () == 0) {

x += 100;

if (fork() == 0) {

x += 50;

print (x);

}

else {

exec (“/bin/ls”); // execute the ls program

print (x)

}

print(x)

}

print(x)

}




1

Q5. Write a C program in Linux  that will create 2 child processes. One child will execute “ps aux” command and the other child will execute “ls -al” command. The child processes will run concurrently. Parent will wait for them until they terminate. You will use fork, exec,  and wait system calls.  There are various versions of the exec system call, such as  execv, execl, execlp, etc. You can use the one that you want.




Q6. Write a C program that will create two children. One child will send “<em>I hear and I forget. I see and I remember. I do and I understand</em>.” string to the other child. The other child will receive the string and will print that out. String will be sent over a message queue.




Q7. Write a C program that will copy a file byte by byte to another file in this manner: every byte in the input file will be duplicated to the output file. If, for example,  input is ‘AB’, the output will be ‘AABB’. Use open(), read(), write(), close() functions (systems calls).


