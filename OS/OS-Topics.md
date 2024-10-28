# OS Topics

## Module 1
1. OS functions:
    - Process Management
    - Memory Management
    - File System Management
    - Device Management
    - Security and Access Control
    - User Interface
    - Networking
    - Resource Allocation and Management
2. Software:
    - Collection of Programs, Instructions and Data
    - To perform specific Tasks
3. Application Software vs System Software

| Aspect          | Application Software                         |  System Software |
|-----------------|----------------------------------------------|------------------|
| **Purpose**     | Directly Perform Specific Tasks for the user | Operate and Manage resources for the System |
| **Dependency**  | Dependent on System Software                 | Independent of Application Software |
| **Examples**    | Word, Excel, Chrome, Photoshop               | Windows, MacOS, Linux, Drivers |

5. Assembler:
    - Translates Assembly code to Machine code
6. Compiler:
    - Translates High level langugues into either Assembly code or Directly to Machine code
7. Interpreter:
    - Directly executes code
    - Line by line translation of code
    - Complied to bytecode sometimes

## Module 2
1. Process:
    - Series of action, steps or operations performed to achieve a specific Task
2. Process Management:
    - Managing and Handling execution of running programs or processes
    - Process Creation and Termination
    - Process Scheduling
    - Process states and transition: new, ready, waiting, running states
    - Inter-Process Communication (IPC): pipes, semaphores, shared memory
    - Process Synchronization and Concurrency: To prevent race conditions and deadlocks
    - Resource Allocation
3. Process Control Block Structure (Diagram):

<table>
<tr>
<td>Process ID (PID)</td>
</tr>          

<tr>
<td>Process State</td>
</tr>

<tr>
<td>Program Counter</td>
</tr>

<tr>
<td>CPU Registers</td>
</tr>

<tr>
<td>Memory Management Info</td>
</tr>

<tr>
<td>I/O Status Info</td>
</tr>

<tr>
<td>Accounting Information</td>
</tr>
</table>

4. States of Process (Diagram):

```
+------------+      +-----------+
|            |      |           |
|    New     +----->+   Ready   |
|            |      |           |
+------+-----+      +-----+-----+
       |                  |
       |                  | (Scheduler allocates CPU)
       |                  |
       |                  v
       |            +-----+-----+
       |            |           |
       |            |  Running  |
       |            |           |
       |            +-----+-----+
       |                  |
       |                  | (I/O request, wait for resource)
       |                  |
       |                  v
       |            +-----+-----+
       |            |           |
       +----------->+  Waiting  |
                    |           |
                    +-----+-----+
                          |
                          | (I/O completed)
                          |
                          v
                    +-----+-----+
                    |           |
                    |   Ready   |
                    |           |
                    +-----+-----+
                          |
                          | (Scheduler allocates CPU)
                          |
                          v
                    +-----+-----+
                    |           |
                    |  Running  |
                    |           |
                    +-----+-----+
                          |
                          | (Process terminates)
                          |
                          v
                    +-----+-----+
                    |           |
                    | Terminated|
                    |           |
                    +-----------+

```

5. CPU Schedulers:
    - Determines how processes are assigned to CPU for execution
    - Maximize CPU ultilization
    - Minimize latency
    - Ensures processes are executed efficiently
    ### 3 States:
    - Ready: Process that are ready to run and waiting for CPU time
    - Running: Currently executing process
    - Blocked: Processes that are waiting for some event to complete before they can continue executing
6. Scheduling Algorithms (Diagram):

    <img src="./FCFS.png" alt="FCFS Chart" width="600" height="300">

    ### Algorithm:
    - Input the processes along with their burst time
    - Find waiting time for all processes
    - As first process that comes need not to wait so waiting time for process 1 will be 0
    - Find waiting time for all other processes, Waiting Time = (Turn Around Time – Burst Time)
    - Find turnaround time = waiting time + burst time for all processes
    - Find average waiting time = total waiting time / no of processes
    - Find average turnaround time = total turn around time / no of processes
7. Resource Allocation (Graph)
8. Deadlock
9. Process Synchronization

## Module 3
1. Memory Management
2. Memory Management Schemes
3. Memory Management Techniques
4. Memory Allocation Strategies
5. Address Binding Schemes
6. Page Replacement Algorithms

## Module 4
1. File System
2. File Operations
3. Types of File Organizations
4. File Organization Algorithm
5. Disk Scheduling Algorithm
6. Classify Directory Structures
7. File Allocation Methods

