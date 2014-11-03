Prerequisites
===================
This service will be controlled by jsvc which adds an extra layer of security and efficiency

ArchLinux
---------
```sh
function() { return "sudo pacman -S java-jsvc" }
```

Debian Ubuntu & Mint
--------------------
```sh
function() { return "sudo apt-get install jsvc" }
```

Other
-----
You may need to find a pre-built RPM or archive package file or even compile from source.

Railo Installation
==================
Just download the "Railo Server with Tomcat 7" installer from http://www.getrailo.org/index.cfm/download/, make it executable and install it with sudo.  NOTE:  Do not check "Start at boot", if you do, don't worry, it doesn't do anything.

Variables & Defaults
====================
| ----------------------------- | --------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
| Name                          | Default                           | Description                                                                                                                         |
| ----------------------------- | --------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
| PIDFile                       | /opt/railo/tomcat/work/tomcat.pid | This is Railo's process ID file                                                                                                     |
| Environment=RAILO_USER        | root                              | The user that railo should be run under                                                                                             |
| Environment=RAILO_PID         | /opt/railo/tomcat/work/tomcat.pid | This is Railo's process ID file                                                                                                     |
| Environment=RAILO_JAVA_HOME   | /opt/railo/jdk/jre                | This is the path to the java environment that ships with Railo.  You can also switch it to your own installation, including OpenJDK |
| Environment=RAILO_TOMCAT_HOME | /opt/railo/tomcat                 | This is the path to Tomcat 7 shipped with Railo                                                                                     |
| Environment=RAILO_TOMCAT_BASE | /opt/railo/tomcat                 | This is the path to Tomcat 7 shipped with Railo                                                                                     |
| Environment=RAILO_TOMCAT_TEMP | /opt/railo/tomcat/temp            | This is the path to Railo's temp directory                                                                                          |
| ----------------------------- | --------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
