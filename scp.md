# Linux scp Command
-------------------
### Command Introduction (命令介绍)
> **SYNOPSIS**
### Command Format and Options (命令格式和选项)
```
#scp --help
unknown option -- -
usage: scp [-12346BCpqrv] [-c cipher] [-F ssh_config] [-i identity_file]
           [-l limit] [-o ssh_option] [-P port] [-S program]
           [[user@]host1:]file1 ... [[user@]host2:]file2
```
### Command Example (命令范例)
```

  scp

  Secure copy.
  Copy files between hosts using Secure Copy Protocol over SSH.

  - Copy a local file to a remote host:
    scp path/to/local_file remote_host:path/to/remote_file

  - Copy a file from a remote host to a local directory:
    scp remote_host:path/to/remote_file path/to/local_directory

  - Recursively copy the contents of a directory from a remote host to a local directory:
    scp -r remote_host:path/to/remote_directory path/to/local_directory

  - Copy a file between two remote hosts transferring through the local host:
    scp -3 host1:path/to/remote_file host2:path/to/remote_directory

  - Use a specific username when connecting to the remote host:
    scp path/to/local_file remote_username@remote_host:path/to/remote_directory

  - Use a specific ssh private key for authentication with the remote host:
    scp -i ~/.ssh/private_key local_file remote_host:/path/remote_file


```
