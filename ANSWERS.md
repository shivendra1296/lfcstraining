This shows possible ways to achieve the tasks described in [README](README.md).

####Table of Contents

1. [Command line](#command-line)
2. [Filesystem and storage](#filesystem-and-storage)
3. [Local system administration](#local-system-administration)
4. [Local security](#local-security)
5. [Shell scripting](#shell-scripting)
6. [Software management](#software-management)

# Command line
## Editing text files on the command line
## Manipulating text files from the command line
1. user accounts
  * ```cut -d':' -f1,7 /etc/passwd > users-shells```
  * ```cut -d':' -f7 /etc/passwd | uniq > shells```
  * ```cut -d':' -f7 /etc/passwd | uniq -c | sort -n -r > shells```
2. ubuntu releases
  * ```wget https://en.wikipedia.org/wiki/List_of_Ubuntu_releases -O ubuntu-releases-web```
  * ```grep -o '<span>.*</span>' ubuntu-releases-web | sed -n 4,23p | cut -d'>' -f2 | cut -d'<' -f1 > ubuntu-releases```
  * ```wc -l ubuntu-releases```

# Filesystem and storage
## Archiving and compressing files and directories
## Assembling partitions as LVM devices
## Configuring swap partitions
## File attributes
## Finding files on the filesystem
## Formatting filesystems
## Mounting filesystems automatically at boot time
## Mounting networked filesystems
## Partitioning storage devices
## Troubleshooting filesystem issues

# Local system administration
## Creating backups
## Creating local user groups
## Managing file permissions
## Managing fstab entries
## Managing local users accounts
## Managing the startup process and related services
## Managing user accounts
## Managing user account attributes
## Managing user processes
## Restoring backed up data
## Setting file permissions and ownership

# Local security
## Accessing the root account
## Using sudo to manage access to the root account

# Shell scripting
## Basic bash shell scripting

# Software management
## Installing software packages