# Linux lpcrm Command
-------------------
### Command Introduction (命令介绍)
> **ipcrm - remove certain IPC resources**
### Command Format and Options (命令格式和选项)
```
#lpcrm --help
-a, --all [shm] [msg] [sem]
          Remove all resources.  When an option argument is provided,
          the removal is performed only for the specified resource
          types.  Warning!  Do not use -a if you are unsure how the
          software using the resources might react to missing objects.
          Some programs create these resources at startup and may not
          have any code to deal with an unexpected disappearance.

   -M, --shmem-key shmkey
          Remove the shared memory segment created with shmkey after the
          last detach is performed.

   -m, --shmem-id shmid
          Remove the shared memory segment identified by shmid after the
          last detach is performed.

   -Q, --queue-key msgkey
          Remove the message queue created with msgkey.

   -q, --queue-id msgid
          Remove the message queue identified by msgid.

   -S, --semaphore-key semkey
          Remove the semaphore created with semkey.

   -s, --semaphore-id semid
          Remove the semaphore identified by semid.

   -V, --version
          Display version information and exit.

   -h, --help
          Display help text and exit.
```
### Command Example (命令范例)
```
	lpcrm

	- To remove the shared memory segment associated with SharedMemoryID 18602, enter:
		ipcrm -m 18602Copy
	- To remove the message queue that was created with a key of 0xC1C2C3C3, enter:
		ipcrm -Q 0xC1C2C3C4
```
