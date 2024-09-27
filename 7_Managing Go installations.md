# Managing Go Installations

## Overview

This guide provides commands to install multiple versions of Go and uninstall Go on macOS/Linux and Windows.

## Table of Commands

| **Task**                              | **macOS/Linux Terminal Commands**                                                | **Windows Command Prompt Commands**                             |
|---------------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------|
| **Install Specific Go Version**      | ```go install golang.org/dl/go1.10.7@latest```                      | ```go install golang.org/dl/go1.10.7@latest```      |
| **Download Installed Version**        | ```go1.10.7 download```                                             | ```go1.10.7 download```                             |
| **Run Command with New Version**     | ```go1.10.7 version```                                             | ```go1.10.7 version```                              |
| **Check Installation Path**           | ```go1.10.7 env GOROOT```                                          | ```go1.10.7 env GOROOT```                           |
| **Remove Go Directory**               | ```sudo rm -rf /usr/local/go```                                    | N/A                                                            |
| **Edit Profile to Remove Go from PATH** | ```nano ~/.profile``` <br> Remove lines with `/usr/local/go/bin` <br> Save and exit | N/A |
| **Reload Profile**                    | ```source ~/.profile```                                            | N/A                                                            |
| **Uninstall via Control Panel**       | N/A                                                                              | Open Control Panel > Programs > Uninstall a program <br> Select "Go Programming Language" and click Uninstall |
| **Uninstall using Command Line**      | N/A                                                                              | ```msiexec /x go{{version}}.windows-{{cpu-arch}}.msi /q``` |

## Notes

- Replace `{{version}}` and `{{cpu-arch}}` in the Windows command with the appropriate version and architecture for your Go installation.
- For macOS/Linux commands, ensure you have appropriate permissions for actions that require `sudo`.

## Conclusion

By following the commands in this guide, you can effectively manage your Go installations across different operating systems. If you encounter any issues, please refer to the official Go documentation or community for assistance.
