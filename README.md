# Buffer-Overflow-Attack
One of cyber attacks is using the buffer overflow. In this project, you are required to design the overflowed buffer to simulate the attack.Then,draw the stack memory allocation graph to show the stack memory of the function foo() in executing target code (before running the line : strcpy(buf); in foo() function).

Objective:

You need to complete the coding of the attack program (exploit.c) to obtain a shell by exploiting stack overflow vulnerability of a given target application (target.c). In reality, if this target application is running on a server accepting remote user input, you can use your exploit code to obtain a command shell (most likely to have root privilege) on the remote server without any password.

 This project is modified from the programming project 1 in U. Berkley’s Dr. Dawn Song’s course “CS161: computer security” in Fall 2008:

http://inst.eecs.berkeley.edu/~cs161/fa08/ 

 Target

The target (target.c) is a simple application which copies the command-line parameter into its own internal buffer stored on the stack. The source code is provided for your reference. Of course you can build your own target while working on the assignment, but the submitted code MUST use the prebuilt target.c.

 Exploit

The exploit is the application (exploit.c) which calls the target (executable program) and passes in an artfully crafted character buffer which causes the target program to give you a shell.
