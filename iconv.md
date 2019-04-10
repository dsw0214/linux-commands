# Linux iconv Command
-------------------
### Command Introduction (命令介绍)
> ****
### Command Format and Options (命令格式和选项)
```
#iconv --help
Usage: iconv [OPTION...] [FILE...]
Convert encoding of given files from one encoding to another.

 Input/Output format specification:
  -f, --from-code=NAME       encoding of original text
  -t, --to-code=NAME         encoding for output

 Information:
  -l, --list                 list all known coded character sets

 Output control:
  -c                         omit invalid characters from output
  -o, --output=FILE          output file
  -s, --silent               suppress warnings
      --verbose              print progress information

  -?, --help                 Give this help list
      --usage                Give a short usage message
  -V, --version              Print program version

Mandatory or optional arguments to long options are also mandatory or optional
for any corresponding short options.

For bug reporting instructions, please see:
<http://www.gnu.org/software/libc/bugs.html>.
```
### Command Example (命令范例)
```

  iconv

  Converts text from one encoding to another.

  - Convert file to a specific encoding, and print to stdout:
    iconv -f from_encoding -t to_encoding input_file

  - Convert file to the current locale's encoding, and output to a file:
    iconv -f from_encoding input_file > output_file

  - List supported encodings:
    iconv -l


```
