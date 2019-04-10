# Linux zip Command
-------------------
### Command Introduction (命令介绍)
> **zip - package and compress (archive) files**
### Command Format and Options (命令格式和选项)
```
#zip --help
Copyright (c) 1990-2008 Info-ZIP - Type 'zip "-L"' for software license.
Zip 3.0 (July 5th 2008). Usage:
zip [-options] [-b path] [-t mmddyyyy] [-n suffixes] [zipfile list] [-xi list]
  The default action is to add or replace zipfile entries from list, which
  can include the special name - to compress standard input.
  If zipfile and list are omitted, zip compresses stdin to stdout.
  -f   freshen: only changed files  -u   update: only changed or new files
  -d   delete entries in zipfile    -m   move into zipfile (delete OS files)
  -r   recurse into directories     -j   junk (don't record) directory names
  -0   store only                   -l   convert LF to CR LF (-ll CR LF to LF)
  -1   compress faster              -9   compress better
  -q   quiet operation              -v   verbose operation/print version info
  -c   add one-line comments        -z   add zipfile comment
  -@   read names from stdin        -o   make zipfile as old as latest entry
  -x   exclude the following names  -i   include only the following names
  -F   fix zipfile (-FF try harder) -D   do not add directory entries
  -A   adjust self-extracting exe   -J   junk zipfile prefix (unzipsfx)
  -T   test zipfile integrity       -X   eXclude eXtra file attributes
  -y   store symbolic links as the link instead of the referenced file
  -e   encrypt                      -n   don't compress these suffixes
  -h2  show more help
  
```
### Command Example (命令范例)
```

  zip

  Package and compress (archive) files into zip file.

  - Package and compress a directory and its contents, [r]ecursively:
    zip -r compressed.zip /path/to/dir

  - E[x]clude unwanted files from being added to the compressed archive:
    zip -r compressed.zip path/to/dir -x path/to/exclude

  - Archive a directory and its contents with the highest level [9] of compression:
    zip -r -9 compressed.zip /path/to/dir

  - Package and compress multiple directories and files:
    zip -r compressed.zip /path/to/dir1 /path/to/dir2 /path/to/file

  - Create an encrypted archive (user will be prompted for a password):
    zip -e -r compressed.zip path/to/dir

  - Add files to an existing zip file:
    zip compressed.zip path/to/file

  - Delete files from an existing zip file:
    zip -d compressed.zip "foo/*.tmp"

  - Archive a directory and its contents to a multi-part [s]plit zip file (e.g. 3GB parts):
    zip -r -s 3g compressed.zip path/to/dir


```
