How would you go about locating the cause of a stack overflow or watchdog timer reset?
Stack overflow is when the stack's memory is full, and the program still tries to use more.
One of the mean reasons for a stack overflow is recursion, and I would first look for any recursive functions.
Review variables that are not static and where an interrupt can occur in the middle of a task.
Another way is setting up exceptions/flags to determine when there is potential for stack overflow at the end of functions/tasks.
A watchdog timer reset is used to help reset the program/system in case something goes wrong or the program hangs. This is usually done via a register for hardware. 
This is usually done via a register for hardware or can be software-driven.
To locate watchdog timer resets, you must find what could be causing the hangup.
This could be caused by an infinite loop, a component that is not responding, or some data that was not copied right and is still waiting to receive the correct information.
Looking for these in code could take a while. Looking to see where it took place and reviewing the cycles it took before it couldn't reset can help narrow the search.
Adding a software watchdog that can feed it can help narrow the search for a possible hang in the code.
