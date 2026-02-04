# cse4001-asst2-os161-code-reading-jfishbein2022

# **Task 1: **
![Docker Container Error](ErrorWhenCommittingFromContainer.png)

# **Task 2: Answer the following questions**



1. OS/161 needs to be reconfigured every time a new file is added to the system either in `kernel` "land" or `userland`. What the path of the directory where the configuration files are kept? 

   ```shell
   kern/conf/
   ```

2. The `trapframe` data structure describes what is saved on the stack during entry to the exception handler. The address of this data structure is passed as an (input) argument to the various trap/interrupt handlers in the system. What is the path of the directory containing the `trapframe` definition? 

   ```shell
   kern/arch/mips/include/
   ```

3. Which file contains the definition of the system call IDs in OS/161? Write the path to the file (including the filename).

   ```shell
   kern/include/kern/syscall.h
   ```

4. The assembly program `kern/arch/mips/locore/exception-mips1.S` is called when a trap/interrupt occurs. What is the instruction that calls the trap handler (.c program)? Write the instruction. 

   ```shell
   jal mips_trap
   ```

5. What is the path to the file where the function `mips_trap()` is implemented? 

   ```shell
   kern/arch/mips/locore/trap.c
   ```

6. What is the path of the file where the function `mips_trap()` is implemented? 

   ```shell
   kern/arch/mips/locore/trap.c
   ```

7. In the file that contains `mips_trap()`, what is the line number where the system-call handler is invoked? 

   ```shell
   syscall(tf) [Line: 152]
   ```

8. What is the path of the file where the system-call handler is implemented? 

   ```shell
   kern/arch/mips/syscall/syscall.c
   ```

9. What field of `trapframe` is used to pass the ID of the system call being requested to the system-call handler? 

   ```c
   tf_v0
   ```

10. In the system-call handler, which variable indicates whether the system call completed successfully?

    ```c
    err
    ```

11. What value is used to indicate the successful completion of system calls? 

    ```c
    0
    ```

12. In the system-call handler, which variable is used to store the return result of a system call other than its success status? 

    ```c
    retval
    ```

13. What the path of the directory where the implementation (i.e., `.c` files) of system calls are kept? 

    ```c
    kern/syscall/
    ```

14. What are the directories inside `userland/testbin/` ? 

   ![Question 14](Question14.png)

15. What is the goal of the file: `userland/testbin/Makefile`? 

    ```c
    Build and install all test programs
    ```

16. Consider lines 6, 7, and 8 in the file `userland/testbin/forktest/Makefile`. What does each line do? 

    ```c
    PROG=forktest //Defines the name of the executable program

    SRCS=forkfest.c //Specifies the source files

    BINDIR=/testbin //Specifies the directory
    ```
