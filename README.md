# ![alt text](./media/command-prompt-logo.png?raw=true) Command Prompt (CMD) Commands

## Introduction

Welcome to the Command Prompt (CMD) Commands reference! CMD is a powerful command-line interface (CLI) for interacting with the Windows operating system.

This guide lists the CMD commands. Where available, the individual CMD files will provide examples of usage for your reference. Enjoy!

## Commands

### File and Directory Commands:
- `dir` - List files and directories in the current directory.
- `chdir` - Change the current directory.
- `cd` - Shorthand version of the `chdir` command.
- `mkdir` - Create a new directory.
- `md` - Shorthand version of the `mkdir` command.
- `rmdir` - Remove a directory.
- `rd` - Shorthand version of the `rmdir` command.
- `copy` - Copy files or directories.
- `move` - Move files or directories.
- `del` - Delete files.
- `rename` - Rename files or directories.
- `ren` - Shorthand version of the `rename` command.
- `type` - Display the contents of a text file.
- `find` - Search for a specific string in a file.
- `attrib` - Change file attributes.
- `tree` - Display directory structure as a tree.
- `xcopy` - Extended copy command with more options.
- `chkdsk` - Check and repair disk errors.
- `fc` - Compare two files or sets of files.
- `comp` - Compare the contents of two files.
- `robocopy` - Robust file and directory copying tool.
- `sfc` - System File Checker to repair corrupted system files.
- `findstr` - Search for specific strings in files.
- `more` - Display the contents of a text file one page at a time.
- `sort` - Sort the contents of a text file.
- `xcopy /e` - Copy directories and subdirectories, including empty ones.
- `compact` - Compress or decompress files on an NTFS partition.
- `xcaccls` - Backup and restore NTFS permissions.
- `subst` - Associate a drive letter with a directory.
- `deltree` - Delete a directory and its subdirectories.
- `cipher` - Display or alter file encryption on NTFS volumes.
- `fsutil` - File system utility for managing various file system settings.
- `openfiles` - Display or disconnect open shared files and folders.

### Network Commands:
- `ipconfig` - Display network configuration information.
- `ping` - Test network connectivity.
- `tracert` - Trace the route to a remote host.
- `netstat` - Display network statistics.
- `nslookup` - Look up IP addresses and domain names.
- `hostname` - Display or set the computer's hostname.
- `arp` - Display and modify the ARP cache.
- `route` - Display or modify the routing table.
- `telnet` - Connect to remote hosts using Telnet.
- `ftp` - Transfer files to/from remote FTP servers.
- `net` - Manage network resources.
- `netsh` - Network Shell for configuring network-related settings.
- `net use` - Connect or disconnect a computer from shared resources.
- `net view` - Display a list of available network resources.
- `net share` - Create, delete, or manage shared folders.
- `net session` - View and manage network sessions.
- `net time` - Synchronize the computer's time with a network server.
- `netdom` - Domain-related management tool.
- `route print` - Display the routing table with more details.
- `nbtstat` - Display statistics and current connections using NetBIOS over TCP/IP.
- `ipconfig /flushdns` - Flush and reset the DNS resolver cache.
- `ipconfig /release` - Release the current DHCP configuration.
- `ipconfig /renew` - Renew the DHCP configuration.
- `netsh firewall` - Configure the Windows Firewall.
- `netstat -a` - Display all active network connections and listening ports.

### System Information and Management:
- `systeminfo` - Display detailed system information.
- `tasklist` - List running processes.
- `taskkill` - Terminate processes or applications.
- `msconfig` - System Configuration Utility.
- `regedit` - Registry Editor.
- `eventvwr` - Event Viewer.
- `services.msc` - Services management console.
- `shutdown` - Shut down or restart the computer.
- `gpupdate` - Update Group Policy settings.
- `ver` - Display the Windows version.
- `systeminfo` - Display detailed system information.
- `gpresult` - Display Group Policy settings for the current user.
- `powercfg` - Configure power management settings.
- `bcdedit` - Boot Configuration Data Editor for managing boot options.
- `dxdiag` - DirectX Diagnostic Tool for troubleshooting DirectX issues.
- `driverquery` - List installed device drivers.
- `msinfo32` - System Information utility.
- `mmc` - Microsoft Management Console for creating custom management tools.
- `taskmgr` - Task Manager for managing running processes.
- `perfmon` - Performance Monitor for system monitoring.
- `wmic` - Windows Management Instrumentation Command-line tool.
- `schtasks` - Schedule tasks to run at specific times or events.

### User Account Management:
- `net user` - Manage user accounts.
- `net group` - Manage user groups.
- `net localgroup` - Manage local groups.
- `whoami` - Display the current user.
- `runas` - Run a program as another user.
- `control userpasswords2` - User Accounts control panel.

### Disk and Storage Management:
- `diskpart` - Disk Partitioning tool.
- `format` - Format a disk drive.
- `defrag` - Defragment disk drives.
- `diskmgmt.msc` - Disk Management console.
- `cleanmgr` - Disk Cleanup utility.

### Miscellaneous Commands:
- `cls` - Clear the screen.
- `echo` - Display text on the screen.
- `date` - Display or set the system date.
- `time` - Display or set the system time.
- `help` - Get help on commands.
- `color` - Change the console text and background color.
- `assoc` - Display or modify file extension associations.
- `shutdown` - Shutdown or restart the computer.
- `shutdown /s` - Shutdown the computer (immediate).
- `shutdown /r` - Restart the computer (immediate).
- `shutdown /h` - Hibernate the computer (if supported).

## License
The content of this project itself is licensed under the [Creative Commons Attribution-ShareAlike 4.0 International license](https://creativecommons.org/licenses/by-sa/4.0/), and the underlying source code used to format and display that content is licensed under the [MIT license](LICENSE).
