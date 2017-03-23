# dockerVM

**The fastest path to a working Docker Engine VM on VirtualBox**

I created this document, because I found no straight forward method to create a simple VM with the Docker Engine installed.

> This document is designed to show a method of creating the fastest path to a working Docker VM on your laptop, whether *Mac or Windows* based.

Follow these steps:

1. Install VirtualBox from one of these [downloads.](http://www.oracle.com/technetwork/server-storage/virtualbox/downloads/index.html)

2. Download the [Ubuntu Desktop ISO.](https://www.ubuntu.com/download/desktop)

3. In VirtualBox, use the New button <img src=images/new.jpg /> to create a Linux VM.  Give it a name, select Linux for the Type and Ubuntu 64bit for the Version.  Set a memory size of at least 2GB, and click the Create button:

<img src=images/2017-03-21_08-58-53.jpg />

4. Add a disk volume of at least 9GB:

<img src=images/2017-03-21_08-59-04.jpg />

5. Start the VM that you just created in VirtualBox:

<img src=images/2017-03-23_11-01-36.jpg />

6. Use the browse control to navigate to the Ubuntu ISO that you downloaded, and mount it.  Click Start:

<img src=images/2017-03-21_09-01-18new.jpg />

7. Install Ubuntu:

<img src=images/2017-03-21_09-02-18.jpg />

8. Accept install options:

<img src=images/2017-03-21_09-02-34.jpg />

9. Erase disk and install (this erases and installs Ubuntu on the VDI virtual disk of the VM):

<img src=images/2017-03-21_09-03-15.jpg />

10. Set time zone and language:

<img src=images/2017-03-21_09-03-31.jpg />

11. Set login info:

<img src=images/2017-03-21_09-04-38.jpg />

12. Ubuntu is then installed.  Restart the VM when prompted:

<img src=images/2017-03-21_09-11-37.jpg />

13. Log into the VM:

<img src=images/2017-03-21_09-12-57.jpg />

14. Search and access the Terminal:

<img src=images/2017-03-21_09-13-53.jpg />

15. For convenience, run as root:

```
$ sudo -s
```

<img src=images/2017-03-21_09-14-23.jpg />

Then, at the command line:

16. Install curl:

```
$ apt install curl
```

17. Install Docker with curl:

```
$ curl -sSL https://get.docker.com/ | sh
```

18. Verify Docker Engine install and run hello-world:

```
$ docker --version
```

```
$ docker run hello-world
```

<img src=images/2017-03-21_09-23-52.jpg />


**Congratulations, you have a working VM with the latest Docker Engine installed and have run your first container!**

***

> At this point, you can do other things with your VM to add convenience.

* Install Guest Additions CD Image (when the VM is running, access this under Devices from the VirtualBox menu bar):

<img src=images/2017-03-21_09-26-21.jpg />

* Set options to allow copy and paste:

<img src=images/2017-03-21_09-27-33.jpg />

* Set up a volume mount to map to a directory on your laptop to the vm to copy/share files:

<img src=images/2017-03-21_13-06-38.jpg />


