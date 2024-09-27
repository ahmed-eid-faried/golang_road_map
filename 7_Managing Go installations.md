Managing Go Installations
=========================

Overview
--------

This guide explains how to install multiple versions of Go on the same machine and how to uninstall Go.

Installing Multiple Go Versions
-------------------------------

* You can install multiple Go versions to test your code across different versions.
* Ensure you have Git installed.
* Use the following command to install a specific version (e.g., 1.10.7):

$ go install golang.org/dl/go1.10.7@latest
$ go1.10.7 download

* To run commands with the newly installed version, append the version number:

$ go1.10.7 version

* To find the installation location of each version, use:

$ go1.10.7 env GOROOT

* To uninstall a version, remove the directory specified by its GOROOT and the corresponding binary.

Uninstalling Go
---------------

### Linux / macOS / FreeBSD

1. Delete the Go directory, typically located at `/usr/local/go`.
2. Remove the Go bin directory from your PATH by editing `/etc/profile` or `$HOME/.profile`. For macOS, also remove the `/etc/paths.d/go` file.

### Windows

1. Uninstall via Control Panel:
    * Go to Add/Remove Programs, select "Go Programming Language," and click Uninstall.
2. Alternatively, use the command line:

msiexec /x go{{version}}.windows-{{cpu-arch}}.msi /q

4. This method will automatically remove any environment variables created during installation.
