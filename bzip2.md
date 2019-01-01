# Linux bzip2 Command
### Command Introduction (命令介绍)
-------------------
> ** bzip2, bunzip2 - a block-sorting file compressor, v1.0.6
bzcat - decompresses files to stdout
bzip2recover - recovers data from damaged bzip2 files **


### Command Format and Options (命令格式和选项)
```
#bzip2 --help
bzip2, a block-sorting file compressor.  Version 1.0.6, 6-Sept-2010.

   usage: bzip2 [flags and input files in any order]

   -h --help           print this message
   -d --decompress     force decompression
   -z --compress       force compression
   -k --keep           keep (don't delete) input files
   -f --force          overwrite existing output files
   -t --test           test compressed file integrity
   -c --stdout         output to standard out
   -q --quiet          suppress noncritical error messages
   -v --verbose        be verbose (a 2nd -v gives more)
   -L --license        display software version & license
   -V --version        display software version & license
   -s --small          use less memory (at most 2500k)
   -1 .. -9            set block size to 100k .. 900k
   --fast              alias for -1
   --best              alias for -9

   If invoked as `bzip2', default action is to compress.
              as `bunzip2',  default action is to decompress.
              as `bzcat', default action is to decompress to stdout.

   If no file names are given, bzip2 compresses or decompresses
   from standard input to standard output.  You can combine
   short flags, so `-v -4' means the same as -v4 or -4v, &c.
```
### Command Example (命令范例)
-------------------
** A block-sorting file compressor. **

- Compress file:

  ` bzip2 path/to/file_to_compress`

- Decompress file:

  ` bzip2 -d path/to/compressed_file.bz2`

- Decompress to console:

  ` bzip2 -dc path/to/compressed_file.bz2`
  