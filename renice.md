# Linux renice Command
-------------------
### Command Introduction (命令介绍)
> **renice -- alter priority of running processes**
### Command Format and Options (命令格式和选项)
```
#renice --help
usage: renice priority     [[-p] pid ...] [[-g] pgrp ...] [[-u] user ...]
       renice -n increment [[-p] pid ...] [[-g] pgrp ...] [[-u] user ...]
```
### Command Example (命令范例)
```
  # renice                                                                                                                                                                                                        
  Alters the scheduling priority/nicenesses of one or more running processes. Niceness values range from -20 (most favorable to the process) to 19 (least favorable to the process).                            
                                                                                                                                                                                                                
	- Change priority of a running process:                                                                                                                                                            
	  renice -n niceness_value -p pid                                                                     

	- Change priority of all processes owned by a user:

	  renice -n niceness_value -u user                                                                    

	- Change priority of all processes that belong to a process group:                                                                                                                          
	  renice -n niceness_value --pgrp process_group       

```
