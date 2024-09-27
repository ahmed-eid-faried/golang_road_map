# Go Installation Guide

## Download and Install Go

Follow the instructions below to download and install Go for your operating system.

### Download Go

[Download Go](https://golang.org/dl/)

## Installation Steps

| **Operating System** | **Installation Steps** | **Verify Installation** |
|----------------------|------------------------|-------------------------|
| **Mac** | 1. Open the downloaded package file. <br> 2. Follow the prompts to install Go. <br> 3. The package installs Go to `/usr/local/go`. <br> 4. Ensure `/usr/local/go/bin` is in your PATH. Restart Terminal if necessary. | Open a command prompt and type: <br> `$ go version` <br> Confirm the version is printed. |
| **Windows** | 1. Open the downloaded MSI file. <br> 2. Follow the prompts to install Go. <br> 3. By default, Go installs to Program Files. <br> 4. Close and reopen command prompts after installation. | Click Start, type `cmd`, and press Enter. <br> Type: <br> `$ go version` <br> Confirm the version is printed. |
| **Linux** | 1. Remove previous installations: <br> `$ rm -rf /usr/local/go` <br> 2. Extract the downloaded archive: <br> `$ tar -C /usr/local -xzf go1.23.1.linux-amd64.tar.gz` <br> 3. Add `/usr/local/go/bin` to PATH by editing `$HOME/.profile` or `/etc/profile`: <br> `export PATH=$PATH:/usr/local/go/bin` <br> 4. Reload profile: <br> `$ source $HOME/.profile` | Open a command prompt and type: <br> `$ go version` <br> Confirm the version is printed. |

## Additional Resources

For more information on managing Go installations or building from source, refer to the official Go documentation.

## Conclusion

By following these steps, you can successfully download, install, and verify Go on your system. If you encounter any issues, please consult the Go community or documentation for further assistance.
