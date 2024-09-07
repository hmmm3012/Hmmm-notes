# Process Management
You can answer all of these questions after reading this chapter.
<details>
    <summary>Revise questions: </summary>

        - What is process ?
        - What is thread ?
        - What is process descriptor? 
        - How does kernel store process descriptors?  

</details>

## The Process
- A process is more than just an executing program code(text section in Unix). It includes a set of resources such as open files, pending signals, interal kernel data, processor state, a memory address space, one or more threads of execution, and a data section. (I will write a program to show all of these info while running)
- Threads, threads of execution, include unique program counter, process stack, and set of process registers.
- Actually, the kernel schedules individual threads, not processes.

## Process Descriptor and the Task Structure
- The kernel stores the list of processes in a circular doubly linked list called ***task list***. Each element in this task list is a process descriptor.
- ***Process descriptor*** contains all the information about a specific process. 
- In Linux, ```struct task_struct``` definded in ```<linux/sched.h>``` is process descriptor.
![the process desriptor and task list](../imgs/task-list.png)
## Process Creation
## The Linux implementation of Threads
## Process Termination
## Conclusion
