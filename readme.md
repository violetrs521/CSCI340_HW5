#Homework 5
##Violet Smith
## 03/01/2022

### 1. pmap Utility

a) Libraries used:
<ul>
    <li> libnss- Name switch configuration file handles each call to a function in which it retrieves data from a system database.
    </li>
    <li> libc- Libc is used to describe the standard c libraries held in linux.
    </li>
    <li> libdl- Dynamic linking library, is used to provide dynamic linking support. It provides backward compatibility for compilation and runtime enviornments.
    </li>

</ul>

b) Other than the virtual page numbers the two bash programs are identical. The actual addresses are not the same.

### Threads

a) What is the main difference between processes and threads?
Threads share address spaces and processes do not. This makes it a lot easier when trying to share data with threads, processes should be used when tasks are logically separate. Processes have page tables and translation lookaside buffers while threads do not this means processes take longer when context switching.


b) Why would you use multiple threads in a program?


c) Example of a process that has multiple threads: 
The name of the command that is running: gjs
The pid for the process: 1662

For each thread show the (5) thread ID's: <ul> <li> SPID: 1662 </li> <li> SPID: 1665 </li> <li>SPID: 1666 </li> <li> SPID: 1668 </li> <li> SPID: 1669 </li>
    </ul>

### Memory and Concurrency

a) I have to go to at least 900000
b) Read the book page 10 threads intro
c) more cores- less clock speed
