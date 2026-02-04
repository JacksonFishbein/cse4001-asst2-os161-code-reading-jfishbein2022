# cse4001-asst2-os161-code-reading-jfishbein2022

Questions:

# **Task 2: Answer the following questions**



1. OS/161 needs to be reconfigured every time a new file is added to the system either in `kernel` "land" or `userland`. What the path of the directory where the configuration files are kept? 

   ```shell
   TETSTSTSTSTST
   ```

2. The `trapframe` data structure describes what is saved on the stack during entry to the exception handler. The address of this data structure is passed as an (input) argument to the various trap/interrupt handlers in the system. What is the path of the directory containing the `trapframe` definition? 

   ```shell
   
   ```

3. Which file contains the definition of the system call IDs in OS/161? Write the path to the file (including the filename).

   ```shell
   
   ```

4. The assembly program `kern/arch/mips/locore/exception-mips1.S` is called when a trap/interrupt occurs. What is the instruction that calls the trap handler (.c program)? Write the instruction. 

   ```shell
   
   ```

5. What is the path to the file where the function `mips_trap()` is implemented? 

   ```shell
   
   ```

6. What is the path of the file where the function `mips_trap()` is implemented? 

   ```shell
   
   ```

7. In the file that contains `mips_trap()`, what is the line number where the system-call handler is invoked? 

   ```shell
   
   ```

8. What is the path of the file where the system-call handler is implemented? 

   ```shell
   
   ```

9. What field of `trapframe` is used to pass the ID of the system call being requested to the system-call handler? 

   ```c
   
   ```

10. In the system-call handler, which variable indicates whether the system call completed successfully?

    ```c
    
    ```

11. What value is used to indicate the successful completion of system calls? 

    ```c
    
    ```

12. In the system-call handler, which variable is used to store the return result of a system call other than its success status? 

    ```c
    
    ```

13. What the path of the directory where the implementation (i.e., `.c` files) of system calls are kept? 

    ```c
    
    ```

14. What are the directories inside `userland/testbin/` ? 

    ```shell
    
    ```

15. What is the goal of the file: `userland/testbin/Makefile`? 

    ```shell
    
    ```

16. Consider lines 6, 7, and 8 in the file `userland/testbin/forktest/Makefile`. What does each line do? 

    ```shell
    
    ```
