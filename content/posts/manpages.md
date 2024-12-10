+++
title = "Manpages"
description = """The OG Unix documentation"""
draft = false
date = "2024-05-14T12:34:56+0100"
author = "P. Paride Martino"
tags = ["linux", "unix","documentation","manpages"]
categories = ["linux", "documentation"]
+++

>Documentation is like sex: when it is good, it is very, very good; and when it is bad, it is better than nothing.
— Dick Brandon

In the early days of Unix, the system used to come with a printed manual, detailing commands and system functions. As Unix grew, the manual became available inside the system, using the man command. With time, and various revisions and reorganizations, the manual system has become a full documentation system, with chapter going from user commands to administration tools, from system APIs to programming and networking.

And to this day, man pages are the quickest way to read the documentation of a command on a Linux system. Typically, a man page is structure in the following way:

- Name: the name of the command
- Synopsis: a summary of the command’s syntax, including its options, arguments, and usage format
- Description: a more detailed explanation of the command’s functionality, describing its purpose, behavior, and any relevant background information.
- Options: a list of the various command-line options (flags or switches) that can be used with the command, along with descriptions of what each option does
- Arguments: a description of any arguments that the command accepts, along with their meanings and possible values
- Examples: a list of examples of how to use the command in various scenarios, demonstrating its usage with different options and arguments
- Exit status: if applicable, here you find a list of the exit status codes returned by the command and their meanings
- See also: a list of related commands, functions, or documentation that may be useful for further reference or exploration
- Author: sometimes you can find here information about the author or authors of the command
- References: this section may contain references to external sources of information, such as manuals, specifications, or related documentation
- History: you may find this section which provides a brief history of the command, including when it was introduced and any significant changes or updates that have been made over time
- Notes: whatever additional notes or comments about the command
As I mentioned above, manual pages went through lots of reorganization over the years. Nowadays, they are organized in a set number of chapters, or sections. Here the list of standard manual pages sections:

1. User Commands: manual pages for various commands available to regular users.
2. System Calls: syscalls are low-level interfaces between user-level programs and the kernel. This section contains manual pages documenting these system calls, providing details about their usage, arguments, and return values.
3. C Library Functions: documentation for functions provided by the C standard library and other system libraries.
4. Devices and Special Files: device files and special files used by the system. This includes documentation for device drivers, file systems, and other hardware-related components.
5. File Formats and Conventions: documentation for file formats, configuration files, and other conventions used by the system, such as the file formats for /etc/passwd, /etc/fstab, /proc.
6. Games and Demos: documentation for games and demo. This includes documentation for classic Unix games like adventure, rogue, tetris, etc.
7. Miscellaneous: miscellaneous documentation that doesn’t fit into other sections is often placed here. This can include macro packages, conventions, protocols, standards, etc.
8. System Administration commands: manual pages for commands typically used by system administrators for system configuration, maintenance, and troubleshooting. Examples include commands like mount, fsck, shutdown, etc.
9. Kernel Developer’s Manual: documentation primarily aimed at kernel developers. It includes information about kernel interfaces, data structures, kernel modules, etc.
The man pages can be non-trivial to navigate, but there is a command which allows to search the entire man pages collection with ease, the command apropos.

Lastly, many distributions have a web version of the man pages, e.g. Debian has

https://manpages.debian.org/

This makes even easier to find information on a Linux system, especially at the beginning when one could not feel totally at home at the command line.