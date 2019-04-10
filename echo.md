# Linux echo Command
-------------------
### Command Introduction (命令介绍)
> **echo - display a line of text**
### Command Format and Options (命令格式和选项)
```
#man echo
ECHO(1)                                                                            User Commands                                                                           ECHO(1)

NAME
       echo - display a line of text

SYNOPSIS
       echo [SHORT-OPTION]... [STRING]...
       echo LONG-OPTION

DESCRIPTION
       Echo the STRING(s) to standard output.

       -n     do not output the trailing newline

       -e     enable interpretation of backslash escapes

       -E     disable interpretation of backslash escapes (default)

       --help display this help and exit

       --version
              output version information and exit

       If -e is in effect, the following sequences are recognized:

       \\     backslash

       \a     alert (BEL)

       \b     backspace

       \c     produce no further output

       \e     escape

       \f     form feed

       \n     new line

       \r     carriage return

       \t     horizontal tab

       \v     vertical tab

       \0NNN  byte with octal value NNN (1 to 3 digits)

       \xHH   byte with hexadecimal value HH (1 to 2 digits)

       NOTE:  your  shell may have its own version of echo, which usually supersedes the version described here.  Please refer to your shell's documentation for details about the
       options it supports.

       GNU coreutils online help: <http://www.gnu.org/software/coreutils/> Report echo translation bugs to <http://translationproject.org/team/>
```
### Command Example (命令范例)
```

  echo

  Print given arguments.

  - Print a text message. Note: quotes are optional:
    echo "Hello World"

  - Print a message with environment variables:
    echo "My path is $PATH"

  - Print a message without the trailing newline:
    echo -n "Hello World"

  - Enable interpretation of backslash escapes (special characters):
    echo -e "Column 1\tColumn 2"


```
