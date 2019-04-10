# Linux chage Command
-------------------
### Command Introduction (命令介绍)
> **chage - change user password expiry information**
### Command Format and Options (命令格式和选项)
```
#chage --help
Usage: chage [options] LOGIN

Options:
  -d, --lastday LAST_DAY        set date of last password change to LAST_DAY
  -E, --expiredate EXPIRE_DATE  set account expiration date to EXPIRE_DATE
  -h, --help                    display this help message and exit
  -I, --inactive INACTIVE       set password inactive after expiration
                                to INACTIVE
  -l, --list                    show account aging information
  -m, --mindays MIN_DAYS        set minimum number of days before password
                                change to MIN_DAYS
  -M, --maxdays MAX_DAYS        set maximim number of days before password
                                change to MAX_DAYS
  -R, --root CHROOT_DIR         directory to chroot into
  -W, --warndays WARN_DAYS      set expiration warning days to WARN_DAYS
```
### Command Example (命令范例)
```
 chage

  Change user account and password expiry information.

  - List password information for the user:
    chage -l user_name

  - Enable password expiration in 10 days:
    sudo chage -M 10 user_name

  - Disable password expiration:
    sudo chage -M -1 user_name

  - Set account expiration date:
    sudo chage -E YYYY-MM-DD

  - Force user to change password on next log in:
    sudo chage -d 0
```
