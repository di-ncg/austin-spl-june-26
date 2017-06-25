# Maven 3 Installation

## Pre-Requisites

You must have Java already installed in order to install and validate Maven.
You can check this by typing `java -version` on the command line.

## Download the Binary

Go to the [download page](http://maven.apache.org/download.cgi#Files) and select either the `Binary tar.gz archive` or the `Binary zip archive`.

## Extract the Binary

Extract the distribution into your preferred directory such as `/usr/local/apache-maven` for Mac/Linux or `C:\bin`.

## Set `M2` Environment Variables

### Mac/Linux

Open a terminal and set environment variables from the command line, replacing `/usr/local/apache-maven` with the directory that you chose above:

```bash
export M2_HOME=/usr/local/apache-maven/apache-maven-3.5.0
export M2=$M2_HOME/bin
```

### Windows

Set these environment variables through the Control Panel, replacing `C:\bin` with the directory that you chose above:

```bash
M2_HOME=C:\bin\apache-maven-3.5.0
M2=%M2_HOME%\bin
```
## Add Maven to the PATH

### Windows

Append the string `;%M2%` to the PATH system environment variable.

### Mac/Linux

Set the `PATH` directly, or update your shell profile:

```bash
export PATH=$M2:$PATH
```

## Validate `mvn`

At the command line, type the following:

```
mvn -v
```

And you should see the Maven and Java version information displayed.


## More Details

You can read through the Maven web site installation docs here: http://maven.apache.org/install.html
