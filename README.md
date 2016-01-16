# strideScheduler

Implemented stride scheduler in proc.c, which allocates CPU to a process based on the number of tickets initially allotted to that process. Stride value is inversely proportional to the number of tickets, and the process with the lowest pass value--cumulative stride value--is given running time. Hence a process with more tickets is scheduled more running time. 

Additionally, implemented system calls getpinfo and settickets in sysproc.c, the former is used for user to monitor the amount of CPU time allocated, and latter for setting the tickets for a process.

