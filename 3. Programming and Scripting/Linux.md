For a comprehensive search that is case-insensitive, looks for multiple keywords, displays context, and shows line numbers:

grep -i -n -C 2 -E "error|fail|exception" application.log

[grep-by-example.pdf](https://github.com/user-attachments/files/19601834/grep-by-example.pdf)

For example, the following cron job runs a backup script every day at 2:30 AM: 30 2 * * * /path/to/backup-script.sh.

[Linux Command Cheat Sheet.pdf](https://github.com/user-attachments/files/19602134/Linux.Command.Cheat.Sheet.pdf)

🔹 Real-World Use Case
Walmart/ASDA: Uses Linux for data operations and automation via CLI for insights and task automation.

🔹 Why Linux?
Open-source, customizable, secure.

Strong community support and less malware-prone.

Preferred for backend, server, and data center systems.

🔹 Linux Fundamentals
Created by Linus Torvalds in 1991.

Based on Unix, features the GNU Utilities.

Consists of various distributions (distros) using the same kernel.

🔹 Linux Directory Structure
Root (/) is the base of everything.

Key Directories:

/etc – Configuration

/dev – Devices

/tmp – Temp files

/mnt, /media – Mount points

/home – User files

/usr – User-land programs

/var – Logs, mail, spool

/bin, /sbin – Binaries for users/admins

/boot – Bootloader files

/opt – Optional apps

🔹 File System Concepts
"Everything is a file" – includes devices, processes, etc.

Four types of files: ordinary, directories, devices, links (hard & soft).

🔹 Linux User & Security Model
Superuser (root) has all privileges.

Users and groups managed via /etc/passwd and /etc/group.

Discretionary Access Control (DAC) for security.

Processes should not run as root unless needed.

🔹 Linux Commands
Basic Commands: ls, cd, pwd, cat, echo, clear, exit, man

System Info: ps, df, free, uname, cal, date

File Management: mv, rm, mkdir, rmdir, touch

Help: command --help, man, info, man -k

🔹 Shell Scripting
Scripts begin with #!/bin/sh

Used for automation (e.g., sending reminders, system info)

Commands can be stored and executed or scheduled (e.g., cron, at)
