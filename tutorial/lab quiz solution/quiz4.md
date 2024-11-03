### CSCI3150 Fall2024 Lab Quiz 4: Paging

#### Question

The correct statement about storage management is ().

A.Multiple processes share a page table

B.Page tables are stored in memory

C.Paging does not cause internal fragmentation

D.An operating system uses paging to manage memory, the sizes of the divided pages can be different.

#### Solution

2/B.

**Explanations**: 

A.Sharing a page table among multiple processes is considered wrong because it violates the fundamental principles of process isolation and memory protection in modern operating systems.

B.Page tables are stored in memory. This option is correct.

C. Paging storage management have internal fragmentation areas. The unused space within the allocated pages is internal fragmentation.  Memory is partitioned into pages of a fixed size, such as 4 KB, and  the total memory requirement of a process is usually not an exact multiple of the page size. For instance, a process may require 10 KB of memory. So 3 pages are allocated to that process and there will be 2KB internal fragmentation.

D.A very important issue in paging management is how to determine the page size. There are many factors in determining the page size, such as the average size of the process, the length of the page table, etc. Once determined, all pages are of equal length (usually an integer power of 2) to facilitate system management.