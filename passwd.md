# Linux passwd Command
### Command Introduction (命令介绍)
-------------------
> **passwd - update user's authentication tokens**

### Command Format and Options (命令格式和选项)
```
#passwd --help
Usage: passwd [OPTION...] <accountName>
  -k, --keep-tokens       keep non-expired authentication tokens
  -d, --delete            delete the password for the named account (root only)
  -l, --lock              lock the password for the named account (root only)
  -u, --unlock            unlock the password for the named account (root only)
  -e, --expire            expire the password for the named account (root only)
  -f, --force             force operation
  -x, --maximum=DAYS      maximum password lifetime (root only)
  -n, --minimum=DAYS      minimum password lifetime (root only)
  -w, --warning=DAYS      number of days warning users receives before
                          password expiration (root only)
  -i, --inactive=DAYS     number of days after password expiration when an
                          account becomes disabled (root only)
  -S, --status            report password status on the named account (root
                          only)
  --stdin                 read new tokens from stdin (root only)

Help options:
  -?, --help              Show this help message
  --usage                 Display brief usage message
```
### Command Example (命令范例)
-------------------
**Passwd is a tool used to change a user's password.**

- Change the password of the current user:

  ` passwd new_password`

- Change the password of the specified user:

  ` passwd username new_password`

- Get the current status of the user:

  ` passwd -S`

- Make the password of the account blank (it will set the named account passwordless):

  ` passwd -d`
