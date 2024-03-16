##process and package management

#Process Management

Process management is an essential aspect of linux administration. Here’s an overview of some important command:-

1 Viewing Processes
a. `ps`
The `ps` command provides a snapshot of the currently running process on the system.  

![vim](/assets/ps.png)

Let’s breakdown the output:-
    -`PID`(Process ID) : unique numerical identifier for each process.
    -`TTY` Terminal type associated with process
    - `Time` total accumulated CPU time consumed by the process.
    -`CMD` the command that started the process. 

b.top
The `top` command displays information about system resources and  currently running process.

![vim](/assets/top.png)

   Let’s breakdown of this output:-

    - `Uptime` '17:52:21 up 33 min’ : The system has been up and running for 33 minutes.
    - `User` 1 users’ : There is one user currency logged in.
    - 'load average' ‘1.06, 1.18, 1.12’ : The load average represents the average number of processes in the run queue over the last 1,5 and 15 minutes

    • Overall cpu usage:
    • ‘2.8% us’ : User space CPU usage.
    • ‘1.7% sy’ : System (kernel) CPU usage.
    • ‘0.0% ni’ : Nice priority user processes.
    • ‘94.5% id’ : Idle cpu time.

    • MIB Men:
    • ‘15734.3 total’ : total physical memory
    • ‘9869.8 free’ : Free physical memory
    • ‘4412.2 used’: used : used physical memory.
    • ‘2683.1 buff/cache’ : memory used for file system buffers and cache.

         • MIB Swap:
    • 977.0 total’ : Total swap space
    • ‘977.0 free’ : free swap space
    • ‘0.0 used’ : used swap space.
    • ‘11322.1 avail Mem’ : Available memory. 
                            
    • Process Table:-
    • Task: ‘284 total’ : total number of processes.
    • Running: ‘1 running’, Sleeping: ‘283 sleeping’, Stopped:’0 stopped.
    • Zombie: ‘0 zombie’.            
    •  Process List:-
    •  PID     : Process ID.
    • USER  : User who owns the process.
    • PR       : Priority.
    • NI         : Nice value.
    • VIRT     : Virtual memory used.
    • RES      : Resident memory used.
    • SHR      : Shared memory used.
    • S           : Process state (R: Running, S: Sleeping, Z: Zombie, etc.).
    • %CPU    : Percentage of CPU usage by the process.
    • %MEM    : Percentage of RAM usage by the process.
    • TIME+     : Total CPU time consumed by the process.
    • COMMAND: Command that started the process.


    Here are a few highlighted processes:-
    • Xorg: The X server, responsible for handling graphical displays.
    • chrome: Google Chrome browser process.
    • firefox-esr: Firefox browser process.


 2. Killing Processes


        a. kill :- 
    The 'kill' command in Linux is used to send a signal to a process, typically to terminate it. We can use it by specifying the Process ID (PID) of the process you want to terminate, like this: kill 1234 
     For example: if we have to kill firefox which has pid “1387”:-

     `$ sudo kill 1357`
     
    ![vim](/assets/kill.png)


Package Management:
Package management on Linux involves the installation, upgrading, configuration and removal of software packages. Different Linux Distributions use different package management systems. Here are some common package management tools for Debian distribution.

 APT:-
APT is the package management command-line tool used in Debian-based Linux distributions, including Ubuntu. Here are some common apt commands:

• Updating package lists:-
`$ sudo apt-get update`

• Upgrading Installed packages:-
`$ sudo apt-get upgrade -y`

• Installing a package:-
`sudo apt install <package name>`

• Removing a package:
`sudo apt remove <package name>`

   