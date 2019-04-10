# Linux dos2unix Command
-------------------
### Command Introduction (命令介绍)
> **dos2unix - DOS/Mac to Unix and vice versa text file format converter**
### Command Format and Options (命令格式和选项)
```
#dos2unix --help
dos2unix 6.0.3 (2013-01-25)
Usage: dos2unix [options] [file ...] [-n infile outfile ...]
 -ascii                convert only line breaks (default)
 -iso                  conversion between DOS and ISO-8859-1 character set
   -1252               Use Windows code page 1252 (Western European)
   -437                Use DOS code page 437 (US) (default)
   -850                Use DOS code page 850 (Western European)
   -860                Use DOS code page 860 (Portuguese)
   -863                Use DOS code page 863 (French Canadian)
   -865                Use DOS code page 865 (Nordic)
 -7                    Convert 8 bit characters to 7 bit space
 -c, --convmode        conversion mode
   convmode            ascii, 7bit, iso, mac, default to ascii
 -f, --force           force conversion of binary files
 -h, --help            give this help
 -k, --keepdate        keep output file date
 -L, --license         display software license
 -l, --newline         add additional newline
 -m, --add-bom         add UTF-8 Byte Order Mark
 -n, --newfile         write to new file
   infile              original file in new file mode
   outfile             output file in new file mode
 -o, --oldfile         write to old file
   file ...            files to convert in old file mode
 -q, --quiet           quiet mode, suppress all warnings
                       always on in stdio mode
 -s, --safe            skip binary files (default)
 -F, --follow-symlink  follow symbolic links and convert the targets
 -R, --replace-symlink replace symbolic links with converted files
                       (original target files remain unchanged)
 -S, --skip-symlink    keep symbolic links and targets unchanged (default)
 -V, --version         display version number
```
### Command Example (命令范例)
```
  - keep output single file date
    dos2unix -k file

  - keep output multiple file date
    dos2unix -k file1 file2 file3

  - keep output multiple file date and write to old file
    dos2unix -k -o file1 file2 file3

  - keep output multiple file date and write to new file
    dos2unix -k -n oldfile newfile
```
