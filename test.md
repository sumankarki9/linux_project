## Process and Package Management

### Process Management

Process management is an essential aspect of Linux administration. Here’s an overview of some important commands: 

1. **Viewing Processes**
    a. `ps`: Provides a snapshot of the currently running processes on the system.
    
    ![ps](/assets/ps.png)
    
    Let’s break down the output:
    - `PID` (Process ID): unique numerical identifier for each process.
    - `TTY`: Terminal type associated with the process.
    - `Time`: total accumulated CPU time consumed by the process.
    - `CMD`: the command that started the process.

    b. `top`: Displays information about system resources and currently running processes.
    
    ![top](/assets/top.png)
    
    Let’s break down this output:
    - `Uptime` '17:52:21 up 33 min’: The system has been up and running for 33 minutes.
    - `User` 1 user: There is one user currently logged in.
    - `Load average` ‘1.06, 1.18, 1.12’: The load average represents the average number of processes in the run queue over the last 1, 5, and 15 minutes.
    
    **Overall CPU usage:**
    - ‘2.8% us’: User space CPU usage.
    - ‘1.7% sy’: System (kernel) CPU usage.
    - ‘0.0% ni’: Nice priority user processes.
    - ‘94.5% id’: Idle CPU time.
    
    **Memory (MiB):**
    - ‘15734.3 total’: total physical memory.
    - ‘9869.8 free’: Free physical memory.
    - ‘4412.2 used’: used physical memory.
    - ‘2683.1 buff/cache’: memory used for file system buffers and cache.
    
    **Swap (MiB):**
    - ‘977.0 total’: Total swap space.
    - ‘977.0 free’: Free swap space.
    - ‘0.0 used’: Used swap space.
    - ‘11322.1 avail Mem’: Available memory.
    
    **Process Table:**
    - `Task`: ‘284 total’: total number of processes.
    - `Running`: ‘1 running’, `Sleeping`: ‘283 sleeping’, `Stopped`:’0 stopped.
    - `Zombie`: ‘0 zombie’.
    
    **Process List:**
    - `PID`: Process ID.
    - `USER`: User who owns the process.
    - `PR`: Priority.
    - `NI`: Nice value.
    - `VIRT`: Virtual memory used.
    - `RES`: Resident memory used.
    - `SHR`: Shared memory used.
    - `S`: Process state (R: Running, S: Sleeping, Z: Zombie, etc.).
    - `%CPU`: Percentage of CPU usage by the process.
    - `%MEM`: Percentage of RAM usage by the process.
    - `TIME+`: Total CPU time consumed by the process.
    - `COMMAND`: Command that started the process.
    
    **Highlighted processes:**
    - `Xorg`: The X server, responsible for handling graphical displays.
    - `chrome`: Google Chrome browser process.
    - `firefox-esr`: Firefox browser process.

2. **Killing Processes**
    - `kill`: The 'kill' command in Linux is used to send a signal to a process, typically to terminate it. We can use it by specifying the Process ID (PID) of the process you want to terminate, like this: `kill 1234`. For example, if we have to kill Firefox which has PID “1387”: `$ sudo kill 1357`.
    
    ![kill](/assets/kill.png)

### Package Management

Package management on Linux involves the installation, upgrading, configuration, and removal of software packages. Different Linux distributions use different package management systems. Here are some common package management tools for Debian distribution.

**APT (Advanced Package Tool):**
APT is the package management command-line tool used in Debian-based Linux distributions, including Ubuntu. Here are some common apt commands:

- Updating package lists:
`$ sudo apt-get update`

- Upgrading Installed packages:
`$ sudo apt-get upgrade -y`

- Installing a package:
`sudo apt install <package name>`

- Removing a package:
`sudo apt remove <package name>`

   