# Operating Systems & Software

# Batch operating system

- doesn’t interact with the computer directly
- An operator takes similar jobs that have the same requirement and group them into batches

![image.png](Operating%20Systems%20&%20Software%201075301291278018be3ee28375e8dbc0/image.png)

### **Common use cases**

Bank statements, payroll systems (Jobs that have to be done on mass)

## Advantages

- The processors of batch systems know how long the job will take
- Multiple users can share the system
- Idle time for a batch system is less
- Easy to manage large work repeatedly

## Disadvantages

- Hard to debug
- Sometimes costly
- Other jobs have to wait for an unknown time if any job fails

---

# Time sharing operating systems

- Each task is given some time to execute so that all the tasks work smoothly
- Multiple users at one time

**Examples**

Unix, Multics

![image.png](Operating%20Systems%20&%20Software%201075301291278018be3ee28375e8dbc0/image%201.png)

## Advantages

- Each task gets equal opportunity
- Fewer chances of duplication of software
- CPU  idle time can be reduced
- Multiple users at once

## Disadvantages

- Reliability problem
- One must have to take care of the security & integrity of programs and data
- Data communication problem

---

# Real time OS

- Serve real time systems, time interval required to process & respond to inputs is very small, the time interval is called response time

## Use cases

Air traffic control, Traffic lights, Missile systems etc.

## Advantages

- Maximum utilization of devices and more output from resources
- Focus on running applications and less importance to applications in the queue
- Error free
- Best managed memory allocation
- In an embedded system (usually just a chip or small board)

## Hard real-time systems

- Very strict and the smallest delay is unacceptable
- Used for airbags etc.

## Disadvantages

- Limited tasks, few run at the same time
- Use heavy system resources
- Complex algorithms
- Device driver and interrupt signals (needs specific drivers)
- Thread priority is not a good idea as they only do one task

## Soft real-time systems

- Used where the timings need to be less strict
- Used in heart monitors (The difference between a microsecond and half a second isn’t going to change reaction speed of a doctor)

---

# Network operating systems

- Run on a server, providing capability to manage data, users, groups, security apps etc.
- Allow shared access of files, printers, resources etc..
- Usually made up of multiple clients and a server or multiple servers and a switch

![image.png](Operating%20Systems%20&%20Software%201075301291278018be3ee28375e8dbc0/image%202.png)

## Advantages

- Highly stable & centralized servers
- Security concerns are handled through servers
- New technologies and hardware upgrading are easily integrated into the system
- Server access is possible remotely from different locations and types of systems

Examples:

## Disadvantages

- Servers are costly
- User has to depend on a central location for most operations
- Maintenance and updates are required regularly

UNIX, Linux, Windows data centre server (eugh)

---

# Operating system types

## Distributed operating systems

- Run on multiple machines that appear as a single unit
- Used for efficient task distribution and load balancing

For example, Hadoop

## Embedded operating systems

- Designed for specific tasks
- Low power & performance
- Used in nearly all IoT devices

Mostly they are all proprietary, but Linux embedded is also often used

## Multi tasking operating systems

- Multiple tasks running at once on a single processor
- Manages resources and allocates CPU time to various processes

## Mobile operating systems

- Allow the user to run different software on phones, tablets etc.
- Mix of a lighter desktop OS made suitable for a mobile device

# Software

## Utility software

Software used to help manage, control and maintain the computer system and its resources. Most operating systems have built in utility software (disk scan, disk defragmentation) But some utility software can be installed on top of the OS, for example anti-virus, registry cleaners etc.

## Application software

Specific programs that are installed onto a computer or made available via the cloud for end users to perform a range of tasks. Includes graphics and CAD software as well as office suites, such as libre office, and browser software such as Firefox and Chromium

## Code development tools (IDE, Debuggers)

Tools used by programmers when developing software, enabling them to create, maintain and debug the software they develop

### Integrated Development Environment

Software that enables developers to have access to main developer tools in a single central interface. IDE’s will include as minimum: a source code editor, compiler and debugger

They can have various other tools installed based on the type of IDE’s, with some having class and object browsers and hierarchy diagrams

- Source code editor - Form of text editor that makes it easier to write and edit source code
- Compiler - Used to convert source code into a format (Usually machine code) that a computer can execute
- Debugger - Used to test the code and identify potential errors. It can highlight code that contains an error or various lines that couldn’t be executed
- Assembler - Program that converts assembly language (low-level programming code) into machine code
- Linker - Sometimes referred to as a link editor. It’s a program that collects and maintains object files and combines them into a single executable file (program)