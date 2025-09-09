[[Operating system structure UNIT 1]]

*System call is a process in which an application software request services from the operating system's kernel,since the application software cannot access the hardware or critical OS functions directly they use system calls as a controlled gateway*

- It is the interface between the user space and the kernel space 

### Working of System call

* *Program request services* - An application calls a library function  (`printf()`) which internally triggers a System call like `write()`
* *Transition to kernel modules* - A special CPU instruction that switches the CPU from user mode to kernel mode
*  *System call handler Executes* - The kernel identifies the requests service using a system call number and executes the corresponding function
* *Kernel performs Operation* - The kernel interacts with the hardware or system resources `writes data to disk`
* *Return to User mode* - Once the operation is complete The kernel switches the CPU back to user mode and returns the result 
* *Program resumes Execution* - The application  continues running using the returned values