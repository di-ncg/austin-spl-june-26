# Installing the `curl` HTTP Tool

## What is it?

`curl` (sometimes spelled as cURL) is a command-line tool for making HTTP requests (GET, POST, etc.) without needing a web browser.
It's a great way to test out HTTP APIs without having to write any code.

## Check if Already Installed

You may already have curl installed as Linux and Mac usually come with it.
To find out, type the following at a command line:

`curl --version`

If it's installed, you'll see something like this:

```bash
curl 7.51.0 (x86_64-apple-darwin16.0) libcurl/7.51.0 SecureTransport zlib/1.2.8
Protocols: dict file ftp ftps gopher http https imap imaps ldap ldaps pop3 pop3s rtsp smb smbs smtp smtps telnet tftp
Features: AsynchDNS IPv6 Largefile GSS-API Kerberos SPNEGO NTLM NTLM_WB SSL libz UnixSockets
```

If you see something like it (your version may be slightly different), then you're done!
If not, continue below.

## Windows

1. Go to [this link](https://curl.haxx.se/dlwiz/?type=bin&os=Win64&flav=-&ver=-&cpu=x86_64) and download the first zip file that's listed.

1. Unzip the downloaded file and move the curl.exe file to a folder such as `C:\curl` or `C:\bin`.

1. Go to http://curl.haxx.se/docs/caextract.html and download the digital certificate file named `cacert.pem`.

   * Move the `cacert.pem` file to your installation folder and rename it `curl-ca-bundle.crt`.

     (Note: The PEM file contains a bundle of valid digital certificates, which are used to verify the authenticity of secure websites.
     This allows cURL to connect securely to servers via HTTPS using the Secure Sockets Layer (SSL) protocol.)

1. Add the curl folder path to your Windows PATH environment variable so that the curl command is available from any location at the command prompt.

1. Test it out by doing `curl --version` at the command line.

## Linux

If your Linux installation doesn't already have `curl`, use this "wizard" to choose the correct file for your distribution: https://curl.haxx.se/dlwiz/?type=bin.
