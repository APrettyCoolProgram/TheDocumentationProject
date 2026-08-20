<!-- 260501 -->

[The Documentation Project](../README.md) ❭ WSL ❭ WSL Basics

***

<div align="center">

<h1>WSL Basics</h1>

  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="../../.github/logo/dark/256x256.png">
    <source media="(prefers-color-scheme: light)" srcset="../../.github/logo/light/256x256.png">
    <img alt="Fallback image description" src="../../.github/logo/light/256x256.png">
  </picture>

</div>

## Basic commands

The main command to start a WSL distribution is" `wsl ~`.

| Command | Description |
| ------- | --- |
| `wsl --list --online` | See a list of the Linux distributions available through the online store |
| `wsl --list` | See a list of the Linux distributions installed on your machine |
| `wsl --list --verbose` | See a list of the Linux distributions installed on your machine, including the state and WSL version |
| | |
| `wsl --install` | Install WSL and the default Ubuntu distribution of Linux. |
| `wsl --install <Distribution Name>` | Install WSL and a specific Linux distribution.|
| `wsl --set-default <Distribution Name>` | Set the default Linux distribution that WSL commands will use to run |
| `wsl --unregister <DistributionName>` | Unregister a specific Linux distribution |
| | |
| `wsl --shutdown` | Immediately terminates all running distributions and the WSL 2 lightweight utility virtual machine. |
| `wsl --terminate <Distribution Name>` | Terminate the specified distribution |
| | |
| `wsl --export <Distribution Name> <FileName>.vhdx --vhd` | Exports a snapshot of the specified distribution as a new distribution file |
| `wsl --import <Distribution Name> <InstallLocation> <FileName>.vhdx --vhd` | Imports the specified VHDX file as a new distribution |
| | |
| `wsl --status` | See general information about your WSL configuration |
| `wsl --update` | Update WSL to the latest version |
| `wsl --uninstall | Uninstall WSL |
| `wsl --help` | Display help information about WSL commands |

## Mount commands

* `wsl --mount <DiskPath>`  
Attach and mount a physical disk in all WSL2 distributions by replacing <DiskPath> with the directory\file path where the disk is located.
  * `--vhd`: Specifies that <Disk> refers to a virtual hard disk.
  * `--name`: Mount the disk using a custom name for the mountpoint
  * `--bare`: Attach the disk to WSL2, but don't mount it.
  * `--type` <Filesystem>: Filesystem type to use when mounting a disk, if not specified defaults to ext4. This command can also be entered as: wsl --mount -t <Filesystem>.You can detect the filesystem type using the command: blkid <BlockDevice>, for example: blkid <dev/sdb1>.
  * `--partition <Partition Number>`: Index number of the partition to mount, if not specified defaults to the whole disk.

* `wsl --unmount <DiskPath>`  
Unmount a disk given at the disk path, if no disk path is given then this command will unmount and detach ALL mounted disks

## Additional information:

* [WLSUI](https://github.com/octasoft-ltd/wsl-ui)

* [Install](https://learn.microsoft.com/en-us/windows/wsl/install)
* [Setup](https://learn.microsoft.com/en-us/windows/wsl/setup/environment#set-up-your-linux-username-and-password)
* [Basic commands](https://learn.microsoft.com/en-us/windows/wsl/basic-commands)
* [Frequently Asked Questions about Windows Subsystem for Linux](https://learn.microsoft.com/en-us/windows/wsl/faq)

<br>

***

[The Documentation Project](../README.md) ❭ WSL ❭ WSL Basics
