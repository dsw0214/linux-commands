# Linux unzip Command
### Command Introduction (命令介绍)
-------------------
> **unzip - list, test and extract compressed files in a ZIP archive**

### Command Format and Options (命令格式和选项)
```
#unzip --help
UnZip 6.00 of 20 April 2009, by Info-ZIP.  Maintained by C. Spieler.  Send
bug reports using http://www.info-zip.org/zip-bug.html; see README for details.

Usage: unzip [-Z] [-opts[modifiers]] file[.zip] [list] [-x xlist] [-d exdir]
  Default action is to extract files in list, except those in xlist, to exdir;
  file[.zip] may be a wildcard.  -Z => ZipInfo mode ("unzip -Z" for usage).

  -p  extract files to pipe, no messages     -l  list files (short format)
  -f  freshen existing files, create none    -t  test compressed archive data
  -u  update files, create if necessary      -z  display archive comment only
  -v  list verbosely/show version info       -T  timestamp archive to latest
  -x  exclude files that follow (in xlist)   -d  extract files into exdir
modifiers:
  -n  never overwrite existing files         -q  quiet mode (-qq => quieter)
  -o  overwrite files WITHOUT prompting      -a  auto-convert any text files
  -j  junk paths (do not make directories)   -aa treat ALL files as text
  -U  use escapes for all non-ASCII Unicode  -UU ignore any Unicode fields
  -C  match filenames case-insensitively     -L  make (some) names lowercase
  -X  restore UID/GID info                   -V  retain VMS version numbers
  -K  keep setuid/setgid/tacky permissions   -M  pipe through "more" pager
  -O CHARSET  specify a character encoding for DOS, Windows and OS/2 archives
  -I CHARSET  specify a character encoding for UNIX and other archives

See "unzip -hh" or unzip.txt for more help.  Examples:
  unzip data1 -x joe   => extract all files except joe from zipfile data1.zip
  unzip -p foo | more  => send contents of foo.zip via pipe into program more
  unzip -fo foo ReadMe => quietly replace existing ReadMe if archive file newer
```
### Command Example (命令范例)
-------------------
**Extract compressed files in a ZIP archive.**

- Extract zip file(s) (for multiple files, separate file paths by spaces):

  ` unzip file(s)`

- Extract zip files(s) to given path:

  ` unzip compressed_file(s) -d /path/to/put/extracted_file(s)`

- List the contents of a zip file without extracting:

  ` unzip -l file.zip`

- Extract the contents of the file(s) to stdout alongside the extracted file names:

  ` unzip -c file.zip`

- Extract a zip file created in windows, containing files with non-ascii (chinese) filenames:

  ` unzip -O gbk file.zip`
