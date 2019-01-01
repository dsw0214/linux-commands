# Linux crontab Command
### Command Introduction (命令介绍)
-------------------
> **crontab - maintains crontab files for individual users**

### Command Format and Options (命令格式和选项)
```
#crontab --help
crontab: invalid option -- '-'
crontab: usage error: unrecognized option
Usage:
 crontab [options] file
 crontab [options]
 crontab -n [hostname]

Options:
 -u <user>  define user
 -e         edit user's crontab
 -l         list user's crontab
 -r         delete user's crontab
 -i         prompt before deleting
 -n <host>  set host in cluster to run users' crontabs
 -c         get host in cluster to run users' crontabs
 -s         selinux context
 -x <mask>  enable debugging

Default operation is replace, per 1003.2
```
### Command Example (命令范例)
-------------------
**Schedule cron jobs to run on a time interval for the current user.
Job definition format: "(min) (hour) (day_of_month) (month) (day_of_week) command_to_execute".**

- Edit the crontab file for the current user:

  ` crontab -e`

- View a list of existing cron jobs for current user:

  ` crontab -l`

- Remove all cron jobs for the current user:

  ` crontab -r`

- Sample job which runs at 10:00 every day. * means any value:

  ` 0 10 * * * path/to/script.sh`

- Sample job which runs every minute on the 3rd of April:

  ` * * 3 Apr * path/to/script.sh`

- Sample job which runs at 02:30 every Friday:

  ` 30 2 * * Fri path/to/script.sh`
