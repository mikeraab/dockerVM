# dockerVM
the fast path to a working Docker Engine VM on VirtualBox

I created this document, because I found no straightforward method to create a simple VM with the Docker Engine installed.

This document is designed to convey one method of creating the fastest path to a working Docker VM on your laptop, whether that is a Mac or Windows based.

Core steps:

1. Install VirtualBox from one of these [downloads](http://www.oracle.com/technetwork/server-storage/virtualbox/downloads/index.html)

2. Download the [Ubuntu Desktop ISO](https://www.ubuntu.com/download/desktop)

3. Create a new Linux VM, select Ubuntu 64bit in VirtualBox:

<img src=images/2017-03-21_08-58-53.jpg />

4. Add a disk volume:

<img src=images/2017-03-21_08-59-04.jpg />

5. Start the VM and mount the Ubunto ISO:

<img src=images/2017-03-21_09-01-18.jpg />

6. Install Umbuntu:

<img src=images/2017-03-21_09-02-18.jpg />

7. Accept install options:

<img src=images/2017-03-21_09-02-34.jpg />

8. Erase disk and install (this erases and install Ubuntu on the VDI virtual disk of the VM, not your real disk)

<img src=images/2017-03-21_09-03-15.jpg />

9. Set time zone and language:

<img src=images/2017-03-21_09-03-31.jpg />

10. Set login info:

<img src=images/2017-03-21_09-04-38.jpg />

11. Ubuntu is then installed.  Restart the VM when prompted.

<img src=images/2017-03-21_09-11-37.jpg />

12. Log into the VM:

<img src=images/2017-03-21_09-12-57.jpg />

13. Search and access the Terminal:

<img src=images/2017-03-21_09-13-53.jpg />

14. For convenience, run as root:

```
$ sudo -s
```

<img src=images/2017-03-21_09-14-23.jpg />

15. Install CURL:

```
$ apt install curl
```

16. Install Docker:

```
$ curl -sSL https://get.docker.com/ | sh
```

17. Verify Docker and run hello-world:

```
$ docker --version
```

```
$ docker run hello-world
```

<img src=images/2017-03-21_09-23-52.jpg />





