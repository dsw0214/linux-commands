# Linux uname Command
### Command Introduction (命令介绍)
-------------------
> ** uname - print system information **

### Command Format and Options (命令格式和选项)
```
#uname --help
Usage: uname [OPTION]...
Print certain system information.  With no OPTION, same as -s.

  -a, --all                print all information, in the following order,
                             except omit -p and -i if unknown:
  -s, --kernel-name        print the kernel name
  -n, --nodename           print the network node hostname
  -r, --kernel-release     print the kernel release
  -v, --kernel-version     print the kernel version
  -m, --machine            print the machine hardware name
  -p, --processor          print the processor type or "unknown"
  -i, --hardware-platform  print the hardware platform or "unknown"
  -o, --operating-system   print the operating system
      --help     display this help and exit
      --version  output version information and exit

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
For complete documentation, run: info coreutils 'uname invocation'
```
### Command Example (命令范例)
-------------------
**
Print details about the current machine and the operating system running on it.
Note: for additional information about the operating system, try the `lsb_release` command.
**

- Print hardware-related information: machine and processor:

  ` uname -mp`

- Print software-related information: operating system, release number, and version:

  ` uname -srv`

- Print the nodename (hostname) of the system:

  ` uname -n`

- Print all available system information (hardware, software, nodename):

  ` uname -a`
