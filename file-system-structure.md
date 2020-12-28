## /
This is known as "root," the logical beginning of the Linux file system structure.
Every single file path in Linux begins from the root.

## /home
This is where all of the personal files are kept.
The Desktop, Documents, Downloads, Photos, and Videos folders are all stored under the /home/username directory.

## /bin
This is where most of binary files are stored, typically for the Linux terminal commands and core utilities.

## /sbin
Like/bin, except that it’s dedicated to certain commands that can only be run by the root user or the superuser.

## /boot
This is where all the needed files for Linux to boot are kept.
A key point to note is that even when /boot is stored on a different partition, it is still logically located at /boot as far as Linux is concerned.

## /dev
This is where physical devices are mounted, such as hard drives, USB drives, optical drives, and so on.
Typically, system hard drive is mounted under "/dev/sda", whereas USB thumb drive might be mounted under "/dev/sde".
There might be different partitions on the disk: /dev/sda1, /dev/sda2, and so on.
"My Computer" in Windows is the equivalent of /dev in Linux file structure.

## /etc
It is where configuration files are stored. Pronounced "et-see". Some also prefer to spell out
Configurations stored in "/etc" will typically affect all users on the system. In contrast, users can also store configuration files under their own /home folders, which will only affect that particular user.

## /lib
This is where libraries are kept. When installing Linux software packages, additional libraries are also automatically downloaded, and they almost always start with lib-something. These are basically the files needed for programs on Linux to work. Think of this folder as somewhat equivalent to the Program Files folder on Windows, although it’s not exactly the same.
Unlike Windows, libraries can be shared between many different programs, which results in Linux installations typically being much more lightweight than Windows, because typically in Windows, each program needs it’s own library installed, even if it’s redundant and already exists for another program.

## /media
Another place where external devices, such as optical drives and USB can be mounted. This varies between different Linux distros.

## /mnt
This is basically a placeholder folder used for mounting other folders or drives.
Typically this is used for Network locations.

## /opt
Optional software for system that is not already managed by distro’s package manager.

## /proc
The "processes" folder where a lot of system information is represented as files.
It basically provides a way for the Linux kernel to send and receive information from various processes running in the Linux environment.

## /root
This is the equivalent to the /home folder specifically for the root user.

## /tmp
This is where temporary files are stored. They are usually deleted upon shutdown.

## /usr
Contains files and utilities that are shared between users.

## /var
This is where variable data is kept, usually system logs but can also include other types of data as well.
