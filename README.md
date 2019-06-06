# oracle-java-installer

Script to install `jdk-VERSION-linux-x64.tar.gz` on Ubuntu.
You need to download the `jdk-VERSION-linux-x64.tar.gz` file from the Oracle web page.

This script was developed with [java 8 from Oracle](https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html) in mind, but should work with other versions also.

Tested on (K)Ubuntu 18.04 x64


# Usage

Options:

**Install tar.gz file**

```bash
$ ./oracle-java-installer.sh --install jdk-VERSION-linux-x64.tar.gz
```

**Remove** 

```bash
$ ./oracle-java-installer.sh --remove java-VERSION-oraclejdk-amd64"
```

**See current default java instalation**

```bash
$ ./oracle-java-installer.sh --status
```


# Why this script

In order to run the [Autopsy forensic browser](https://www.sleuthkit.org/autopsy/download.php) on Linux you need to install the latest version of java 8 from Oracle. 
Unfortunately, since 2019-04-16 the preferred method for Ubuntu **no longer works**:
```bash
$ sudo add-apt-repository ppa:webupd8team/java
$ sudo apt update
$ sudo apt install oracle-java8-installer
```
You can read more about this [here](https://launchpad.net/~webupd8team/+archive/ubuntu/java).

