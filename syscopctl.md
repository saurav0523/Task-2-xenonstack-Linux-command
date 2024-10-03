# syscopctl(1) - Custom Linux Command

## SYNOPSIS

**syscopctl** [**command**] [**options**]

## DESCRIPTION

The `syscopctl` command is a custom Linux command that provides various functionalities for system management.

## COMMANDS


- **memory getinfo**:
  Get Memory information similar to the `free` command.

- **user create <username>**:
  Create a new user who can log in to the Linux system and access their home directory.

- **user list**:
  List all regular users on the server.

- **user list --sudo-only**:
  List all users with sudo permissions on the server.

- **file getinfo [options] <file-name>**:
  Get information about a file, with optional specific information.



- **free**:
  Display amount of free and used memory in the system.


## OPTIONS

- **--size, -s**:
  Print the size of the specified file.

- **--permissions, -p**:
  Print the file permissions.

- **--owner, -o**:
  Print the file owner.

- **--last-modified, -m**:
  Print the last modified time of the specified file.

## EXAMPLES

```sh
$ syscopctl cpu getinfo
$ syscopctl memory getinfo
$ syscopctl user create myuser
$ syscopctl user list
$ syscopctl user list --sudo-only
$ syscopctl file getinfo /path/to/myfile.txt
$ syscopctl file getinfo --size /path/to/myfile.txt
% syscopctl free
