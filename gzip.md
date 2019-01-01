# Linux gzip Command
### Command Introduction (命令介绍)
-------------------
> ** gzip, gunzip, zcat - compress or expand files **

### Command Format and Options (命令格式和选项)
```
#gzip --help
Usage: gzip [OPTION]... [FILE]...
Compress or uncompress FILEs (by default, compress FILES in-place).

Mandatory arguments to long options are mandatory for short options too.

  -c, --stdout      write on standard output, keep original files unchanged
  -d, --decompress  decompress
  -f, --force       force overwrite of output file and compress links
  -h, --help        give this help
  -l, --list        list compressed file contents
  -L, --license     display software license
  -n, --no-name     do not save or restore the original name and time stamp
  -N, --name        save or restore the original name and time stamp
  -q, --quiet       suppress all warnings
  -r, --recursive   operate recursively on directories
  -S, --suffix=SUF  use suffix SUF on compressed files
  -t, --test        test compressed file integrity
  -v, --verbose     verbose mode
  -V, --version     display version number
  -1, --fast        compress faster
  -9, --best        compress better
    --rsyncable   Make rsync-friendly archive

With no FILE, or when FILE is -, read standard input.

Report bugs to <bug-gzip@gnu.org>.
```
### Command Example (命令范例)
-------------------
** Compress/uncompress files with gzip compression (LZ77). **

- Compress a file, replacing it with a gzipped compressed version:

  ` gzip file.ext`

- Decompress a file, replacing it with the original uncompressed version:

  ` gzip -d file.ext.gz`

- Compress a file specifying the output filename:

  ` gzip -c file.ext > compressed_file.ext.gz`

- Uncompress a gzipped file specifying the output filename:

  ` gzip -c -d file.ext.gz > uncompressed_file.ext`

- Specify the compression level. 1=Fastest (Worst), 9=Slowest (Best), Default level is 6:

  ` gzip -9 -c file.ext > compressed_file.ext.gz`
