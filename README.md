# oracle-java8-installer
Oracle Java 8 packages for Ubuntu/Debian (8u201) - The Oracle JDK License has changed for releases starting April 16, 2019.
Please note that Java 8 reached its end of public updates and Oracle will not release any more updates after January 2019. For details please see https://www.oracle.com/technetwork/java/java-se-support-roadmap.html

Introduction
------------

Oracle Java 8 packages for Ubuntu/Debian.

Supported Ubuntu/Debian versions
-------------------------

So far packages were tested on following Ubuntu versions:

- none

So far packages were tested on following Debian versions:

- none

However, if one finds any problem on others Ubuntu/Debian,
feel free to report an issue and I will try to resolve it.

Usage
-----

To create packages on your own:

- sudo apt install -y debhelper build-essential
- git clone -b 8u201_armhf https://github.com/tod31/oracle-java8-installer.git
- cd oracle-java8-installer
- download jdk-8u201-linux-arm32-vfp-hflt.tar.gz and jce_policy-8.zip
- Link JDK: https://www.oracle.com/technetwork/java/javase/downloads/java-archive-javase8-2177648.html
- Link JCE: https://www.oracle.com/technetwork/java/javase/downloads/jce8-download-2133166.html
- dpkg-buildpackage -uc -us
- install with internet any missing packages that dpkg-buildpackage complains about and repeat
