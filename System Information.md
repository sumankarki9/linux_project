## System Information

There are various commands in Linux to retrieve details about the hardware, operating system, and other relevant information. Here are some commonly used commands:

### a. `uname -a`

`uname -a` command displays detailed system information including the kernel version, hostname, release, architecture, etc.

![uname](/assets/uname.png)

In this output from the ‘uname -a’ command, it provides various details about the Linux system. Here’s the detailed information:
- `Kernel version`: 6.5.0-kali3-amd64
- `Hostname`: suman
- `Kernel Release Date`: Debian 6.5.6-1kali1 (2023-10-09)
- `Architecture`: x86_64
- `GNU/Linux`: GNU project and uses Linux kernel.

### b. `lsb_release -a`

`lsb_release -a` command provides information about the Linux distribution and version.

![lsb_release](/assets/ls_re.png)

### c. `hostname`

`hostname` command displays the name of the host system.

![hostname](/assets/hostname.png)

### d. `cat /etc/os-release`

This command shows the information from the `/etc/os-release` file, including the distribution name, version, and ID.

![os-release](/assets/os-release.png)

### e. `df -h`

This command is used to display information about disk space usage on the Linux system.

![df-h](/assets/df-h.png)

Here’s more information about this output:
- `Filesystem`: Indicates the name of the filesystem.
- `Size`: Represents the total size of the filesystem.
- `Used`: Displays the amount of disk space used.
- `Avail`: Shows the available (free) disk space.
- `Use%`: Indicates the percentage of disk space used.
- `Mounted on`: The directory where the filesystem is mounted.

### f. `free`

The `free` command is used to get information about the system’s memory usage.

![free](/assets/free.png)

Here’s the detailed information about the output (system’s memory usage):
- `total`: Total RAM available in the system (in this case, it’s 16,111,932 KB).
- `used`: Amount of RAM currently in use (in this case, it’s 3,737,252 KB).
- `free`: Amount of free RAM (in this case, it’s 10,896,852 KB).
- `shared`: Used memory that can be shared among multiple processes (in this case, it’s 693,996 KB).
- `buff/cache`: Memory used for filesystem buffers and cache (in this case, it’s 2,482,892 KB).
- `available`: An estimate of how much memory is available for starting new applications, without swapping (in this case, it’s 12,374,680 KB).

### g. `lsblk`

This command is used to list information about block devices (hard drives, SSDs, etc.) on the system.

![lsblk](/assets/lsblk.png)

Here’s the breakdown of the output:
- `sda`: A disk with a total size of 931.5 GB and its contains two partitions:
  - `sda1`: 512 MB in size.
  - `sda2`: 931 GB in size.
- `nvme0n1`: Another disk with a total size mounted at ‘/boot/efi’ and its contains  three partitions:
  - `nvme0n1p1`: 512 MB in size, mounted at ‘/boot/efi’.
  - `nvme0n1p2`: 237 GB in size, mounted at ‘/’.
  - `nvme0n1p3`: 977 MB in size, used as swap space.

### h. `uptime`

The `uptime` command provides information about how long the system has been running.

![uptime](/assets/uptime.png)

Here’s the breakdown of this output:
- `17:35:56`: The current time.
- `up 16 min`: The system has been up and running for 16 minutes.
- `1 user`: There is currently 1 user logged into the system.
- `load average`: 0.85, 1.08, 0.86: The system load averages for the last 1, 5, and 15 minutes, respectively.
