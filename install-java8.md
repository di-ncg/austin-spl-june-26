# Java 8 Installation

Check first to see if you have Java already installed:

1. Open a command prompt or terminal window

1. Type `javac -version`

1. If you see something like:

   ```
   javac 1.8.0_212
   ```

   Then you're all set! If not, continue below.

## Download Page

1. Go to https://adoptopenjdk.net/
1. Select **OpenJDK 8 (LTS)**
1. Click the "Latest Release" button to download.

## Windows

1. Run the file, accepting all defaults from the installer
1. Open up the system environment variables dialog and add the variable `JAVA_HOME` with the value `C:\Program Files\Java\jdk1.8.0_181` (or wherever the JDK was installed if you selected a different location)
1. Edit the system environment variable and **append** to the end `;%JAVA_HOME%\bin`.
1. Open a command prompt and type the following commands to verify it's installed correctly:
   * `javac -version`
   * `java -version`

## Mac OS X

1. Open/launch the `.dmg` file and run the package installer that's inside and follow the directions
1. Open a terminal and type the following commands to verify it's installed correctly:
   * `javac -version`
   * `java -version`

## Linux

1. For the tar.gz format:
   * Untar the file using `tar -xvf <jdk-8u181-linux-x64.tar.gz> -C <destination-directory>`
   * `export JAVA_HOME=<destination-directory>/jdk1.8.0_181`
   * *Append* to the PATH `:$JAVA_HOME/bin`
1. Open a terminal and type the following commands to verify it's installed correctly:
   * `javac -version`
   * `java -version`
