# Java 8 Installation

## Download Page

1. Go to http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html
1. Scroll to the first section, labeled **Java SE Development Kit 8u131**
1. Accept the License Agreement (otherwise you won't be able to select a download)

## Windows

1. Choose the `Windows x64` (*not* x86) file named `jdk-8u131-windows-x64.exe`
1. Run the file, accepting all defaults from the installer
1. Open up the system environment variables dialog and add the variable `JAVA_HOME` with the value `C:\Program Files\Java\jdk1.8.0_131` (or wherever the JDK was installed if you selected a different location)
1. Edit the system environment variable and **append** to the end `;%JAVA_HOME%\bin`.
1. Open a command prompt and type the following commands to verify it's installed correctly:
   * `javac -version`
   * `java -version`

## Mac OS X

1. Choose the `Mac OS X` file named `jdk-8u131-macosx-x64.dmg`
1. Open/launch the `.dmg` file and run the package installer that's inside and follow the directions
1. Open a terminal and type the following commands to verify it's installed correctly:
   * `javac -version`
   * `java -version`

## Linux

1. Choose the rpm or tar.gz file as appropriate for your distribution
1. For the tar.gz format:
   * Untar the file using `tar -xvf <jdk-8u131-linux-x64.tar.gz> -C <destination-directory>`
   * `export JAVA_HOME=<destination-directory>/jdk1.8.0_131`
   * *Append* to the PATH `:$JAVA_HOME/bin`
1. Open a terminal and type the following commands to verify it's installed correctly:
   * `javac -version`
   * `java -version`
