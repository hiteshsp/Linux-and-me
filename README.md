# Linux-and-me

awk, sed, grep, egrep, fgrep --> Text processing/searching commands

grep: searches a specific term in a file
awk and sed are text processors i.e. they can perform operations such as "replace","update" etc.
awk is mostly used for data extraction where sed is a stream editor

##### Sed #####
`sed -i 's/cat/dog/' file.txt` // Replaces cat with dog

##### awk ####
`awk '{print $2}' file.txt` // Prints the second column in the file

"awk" is a complete programming language built around the CSV style files. Not preferred for simple tasks,
whereas "sed" is prominently used for simple tasks like using regex

##### COMMON OPERATIONS #####

| Commands | Description |
| --- | ---|
| `fmt` | text formatter |
| `tr` | translate characters |
| `nl` | number of lines in a file |
| `wc` | word count |

sort, uniq, cut 
 
##### PROCESS COMMANDS #####
| Commands | Description |
| --- | ---|
| `ps` | report a snapshot of the current processes |
| `top` | display Linux processes |
| `htop` | interactive process viewer |
| `lsof` | list open files with pid |

ps, top, htop, atop, lsof 
* htop: top with scroll vertically and horizontally
* atop: similar like top
* lsof: list open files with pid

##### NETWORKING COMMANDS #####

| Commands | Description |
| --- | ---|
| `nmap`| Network exploration tool and security / port scanner |
| `tcpdump` | dumps all the network traffic |
| `ping` | send ICMP ECHO_REQUEST to network hosts |
| `mtr` | a.k.a My traceroute   a network diagnostic tool which combines the functionality of traceroute and ping |
| `traceroute` | print the route packets trace to network host |
| `airmon-ng` |  a bash script designed to turn wireless cards into monitor mode |
| `airodump-ng` | a packet capture tool for aircrack-ng |
| `aircrack-ng` | a 802.11 WEP / WPA-PSK key cracker works on airodump packets |
| `reaver` | WPS Cracker |
| `dig` |  a.k.a domain ingormation groper: DNS lookup utility |
| `vmstat` | Report virtual memory statistics |
| `strace` | trace system calls and signals |
| `dtrace` | Dtrace compatible user application static probe generation tool. |
| `iptables` | administration tool for IPv4/IPv6 packet filter‐ing and NAT |
| `iostat` | Report  Central  Processing  Unit  (CPU)  statistics  and input/output statistics for devices and partitions.  |
| `sar` | Collect, report, or save system activity information. |
| `nmon` | Systems administrator, tuner, benchmark tool. |
nmap, tcpdump, ping, mtr, traceroute, airmon, airodump, dig, iptables
strace, dtrace, systemtap, uname, df

* strace: Strace is a utility that intercepts and logs these system calls. In this way, you can watch how a program interacts with the system, which is useful for tracking down behavioural issues. 
* dtrace: 
* dig a.k.a domain ingormation groper: DNS lookup utility
* mtr : My traceroute
* tcpdump: dumps all the network traffic
* vmstat: 
  It's a computer system monitoring tool that collects and displays summary information about 
        operating system memory
        processes
        interrupts
        paging and block I/O

Systat package for iostat and sar
* iostat 
    It gives you information relevant to cpu util steal time load etc.
* sar - Collect, report, or save system activity information. 
    ```sar is a classic Linux tool that is part of the sysstat package and should be available in just about any major distribution with your regular package manager. Once installed, it will be enabled on a Red Hat-based system, but on a Debian-based system (like Ubuntu), you might have to edit /etc/default/sysstat, and make sure that ENABLED is set to true. On a Red Hat-based system, sar will log seven days of statistics by default. 
    If you want to log more than that, you can edit /etc/sysconfig/sysstat and change the HISTORY option. ```
    It can be used to find the difference between a particular day and now etc.
    Provides CPU, RAM, Turn Back Time, Disk statistics
* nmon
    Its a interactive and visual display of the network monitoring utility
    You can grab info about CPU, Disk, memory etc.
