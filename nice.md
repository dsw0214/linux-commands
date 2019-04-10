# Linux nice Command
-------------------
### Command Introduction (命令介绍)
> **nice -- execute a utility with an altered scheduling priority**
### Command Format and Options (命令格式和选项)
```
#nice 
usage: nice [ -n increment ] utility [ argument ...]
```
### Command Example (命令范例)
```
  # nice                                                                                                                                                                                                          
                                                                                                                                                                                                                
  Execute a program with a custom scheduling priority (niceness).                                                                                                                                               
  Niceness values range from -20 (the highest priority) to 19 (the lowest).                                                                                                                                     
                                                                                                                                                                                                                
- Launch a program with altered priority:                                                                                                                                                                       
                                                                                                                                                                                                                
  nice -n niceness_value command    

```
