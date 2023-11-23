# XV Quiz (CSL 3030)

Welcome to the XV Quiz for CSL 3030 - Operating Systems!



## Instructions
- Answer the multiple-choice questions by selecting the correct option.
- For theoretical questions, provide concise and accurate explanations.
- Feel free to use this quiz for self-assessment or educational purposes.

## Multiple-Choice Questions

#### Question 1: Basics
1. What is XV6?
   - a. A programming language
   - b. A Unix-like operating system
   - c. A file system
   - d. An assembly language

#### Question 2: Architecture
2. XV6 is based on which earlier operating system?
   - a. Windows
   - b. Linux
   - c. BSD
   - d. DOS

#### Question 3: File System
3. Which file system is used in XV6?
   - a. FAT32
   - b. NTFS
   - c. ext4
   - d. simple

#### Question 4: System Calls
4. How are system calls implemented in XV6?
   - a. As functions in the C standard library
   - b. As interrupts
   - c. Through the command line
   - d. As external programs

#### Question 5: Processes
5. In XV6, what is the maximum number of processes that can run simultaneously?
   - a. 128
   - b. 256
   - c. 512
   - d. 1024

#### Question 6: Shell
6. What is the name of the shell used in XV6?
   - a. Bash
   - b. Zsh
   - c. Sh
   - d. Fish

#### Question 7: Scheduling
7. How does XV6 handle process scheduling?
   - a. Round-robin scheduling
   - b. Priority-based scheduling
   - c. First-Come-First-Serve (FCFS)
   - d. Random scheduling

#### Question 8: Memory Management
8. Which memory management technique is used in XV6?
   - a. Paging
   - b. Segmentation
   - c. Virtual Memory
   - d. None of the above

#### Question 9: Interrupts
9. How are interrupts handled in XV6?
   - a. Through polling
   - b. Using hardware interrupts
   - c. Using software interrupts
   - d. Both b and c

#### Question 10: Multithreading
10. Does XV6 support multithreading?
    - a. Yes
    - b. No

#### Bonus Question:
11. Who developed XV6?
    - a. Microsoft
    - b. Google
    - c. MIT
    - d. IBM

## Theoretical Questions

#### Question 12: Process States
12. Briefly explain the different states a process can be in within the XV6 operating system.

#### Question 13: File System Structure
13. Describe the structure of the file system in XV6. Include the key components and their roles.

#### Question 14: System Calls vs. Library Functions
14. Explain the difference between system calls and library functions in the context of XV6. Provide examples of each.

#### Question 15: Memory Paging
15. How does memory paging work in XV6? Discuss the benefits of using paging in memory management.

#### Question 16: Shell Commands
16. Name and briefly explain three essential shell commands in the XV6 operating system.

#### Question 17: Process Synchronization
17. Discuss the concept of process synchronization in XV6. Why is it essential, and what mechanisms are used to achieve it?

#### Question 18: Interrupt Handling
18. Explain the role of interrupts in the XV6 operating system. How are interrupts handled, and what is their significance in system operation?

#### Question 19: Virtual Memory
19. What is virtual memory, and how is it implemented in XV6? Discuss the advantages of using virtual memory.

#### Question 20: Boot Process
20. Outline the steps involved in the boot process of XV6. What happens from the moment the computer is powered on to when the XV6 kernel is loaded into memory?

## Answers
1. B(A Unix-like operating system)
2. C(BSD)
3. D(simple)
4. B(As interrupts)
5. A(128)
6. C(Sh)
7. A(Round-robin scheduling)
8. A(Paging)
9. D(Both b and c)
10. B(No)
11. C(MIT)
12. In XV6 Operating System, A process can be in different states such as :
    1. Running:
       Process actively using the CPU.
       Executing its instructions.

   2. Sleeping:
      Waiting for an event (e.g., I/O completion).
      
   3. Zombie:
      Process has terminated but still has an entry in the process table.
      
   4. Unused:
      Process table entry not in use.
      
   5. Embryo:
      Newly created process.
      
   6. Wait:
      Process waiting for its child to exit.
      Typically, waiting in the wait() system call.
      
13. XV6 utilizes a hierarchical file system architecture, similar to that of Unix, with directories, files, and Inodes. Inodes serve the purpose of storing metadata pertaining to files and the locations of 
    their data blocks.

14. System calls are interfaces between user-level applications and the operating system kernel. They provide a way for applications to request services from the operating system while Library functions are 
    precompiled routines that applications can use. They are not part of the operating system kernel but are linked with the application at compile or runtime.

    Examples of System Calls()
    fork(): Creates a new process.
    exit(): Terminates the calling process.
    read(): Reads data from a file descriptor.
    
    Examples of Library functions()
    printf(): Prints formatted output to the standard output.
    malloc(): Allocates a specified number of bytes of memory.
    strlen(): Returns the length of a string.
    
15. Memory paging in XV6 involves breaking physical memory into fixed-size blocks (pages). Paging enhances memory utilization and simplifies management.

16. The three essential shell commands in the XV6 operating system :
    ls- Lists all files in a given directory
    cd- Changes the current directory to open a new directore.
    echo- Print something directly to the terminal.

17. Process synchronization in XV6 is used to prevent conflicts and ensure data consistency. Mechanisms like mutex locks, semaphores, and conditional variables are used.
18. Interrupts in XV6 are managed through interrupt service routines (ISRs) and the interrupt descriptor table (IDT). They play a vital role in handling external events and ensuring timely system responses.
19. Virtual memory  allows processes to use more memory than physically available, generally implemented through paging. This provides benefits such as process isolation ,  effective paging and efficient memory 
    utilization.
20. The XV6 boot process involves hardware initialization, bootloader loading (e.g., GRUB), kernel loading into memory, and control transfer to the kernel. The kernel then initializes the system, mounts the 
    root file system, and starts the init process.
