# Linux umask Command
-------------------
### Command Introduction (命令介绍)
> **bash, :, ., [, alias, bg, bind, break, builtin, caller, cd, command, compgen, complete, compopt, continue, declare, dirs, disown, echo, enable, eval, exec, exit, export,**
### Command Format and Options (命令格式和选项)
```
umask: usage: umask [-p] [-S] [mode]
```
### Command Example (命令范例)
```

  umask

  Manage the read/write/execute permissions that are masked out (i.e. restricted) for newly created files by the user.

  - Display the current mask in octal notation:
    umask

  - Display the current mask in symbolic (human-readable) mode:
    umask -S

  - Change the mask symbolically to allow read permission for all users (the rest of the mask bits are unchanged):
    umask a+r

  - Set the mask (using octal) to restrict no permissions for the file's owner, and restrict all permissions for everyone else:
    umask 077


```
