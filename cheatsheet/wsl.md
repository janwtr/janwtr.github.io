# Cheat Sheet Windows Subsystem for Linux (WSL)
## Arguments for running Linux commands
Command | Description
-------:|------------
``wsl`` (Without arguments) | If no command line is provided, wsl.exe launches the default shell.
``wsl --exec, -e <CommandLine>`` | Execute the specified command without using the default Linux shell.
``wsl --distribution, -d <Distro>`` | Run the specified distribution.
``wsl --user, -u <UserName>`` | Run as the specified user.

## Arguments for managing Windows Subsystem for Linux
Command | Description
-------:|------------
``wsl --export <Distro> <FileName>`` | Exports the distribution to a tar file. The filename can be - for standard output.
``wsl --import <Distro> <InstallLocation> <FileName>`` | Imports the specified tar file as a new distribution. The filename can be - for standard input.
``wsl --list, -l [Options]`` | Lists distributions. Options: ``--all``, List all distributions, including distributions that are currently being installed or uninstalled.
``wsl --running`` | List only distributions that are currently running.
``wsl --set-default, -s <Distro>`` | Sets the distribution as the default.
``wsl --terminate, -t <Distro>`` | Terminates the specified distribution.
``wsl --unregister <Distro>`` | Un-register the distribution.
``wsl --help`` | Display usage information.
