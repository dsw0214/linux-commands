# Linux bc Command
-------------------
### Command Introduction (命令介绍)
> **bc - An arbitrary precision calculator language**
### Command Format and Options (命令格式和选项)
```
#bc --help
usage: bc [options] [file ...]
  -h  --help         print this usage and exit
  -i  --interactive  force interactive mode
  -l  --mathlib      use the predefined math routines
  -q  --quiet        don't print initial banner
  -s  --standard     non-standard bc constructs are errors
  -w  --warn         warn about non-standard bc constructs
  -v  --version      print version information and exit
```
### Command Example (命令范例)
```

  bc

  Calculator.

  - Run calculator in interactive mode using the standard math library:
    bc -l

  - Calculate the result of an expression:
    bc <<< "(1 + 2) * 2 ^ 2"

  - Calculate expression and force number of decimal places to 10:
    bc <<< "scale=10; 5 / 3"

  - Calculate expression with sine and cosine using mathlib:
    bc -l <<< "s(1) + c(1)"


```
