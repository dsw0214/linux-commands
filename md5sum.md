# Linux md5sum Command
-------------------
### Command Introduction (命令介绍)
> **dgst, sha, sha1, mdc2, ripemd160, sha224, sha256, sha384, sha512, md2, md4, md5, dss1 - message digests**
### Command Format and Options (命令格式和选项)
```
#md5sum --help
Usage: md5sum [OPTION]... [FILE]...
Print or check MD5 (128-bit) checksums.
With no FILE, or when FILE is -, read standard input.

  -b, --binary         read in binary mode
  -c, --check          read MD5 sums from the FILEs and check them
      --tag            create a BSD-style checksum
  -t, --text           read in text mode (default)
  Note: There is no difference between binary and text mode option on GNU system.

The following four options are useful only when verifying checksums:
      --quiet          don't print OK for each successfully verified file
      --status         don't output anything, status code shows success
      --strict         exit non-zero for improperly formatted checksum lines
  -w, --warn           warn about improperly formatted checksum lines

      --help     display this help and exit
      --version  output version information and exit

The sums are computed as described in RFC 1321.  When checking, the input
should be a former output of this program.  The default mode is to print
a line with checksum, a character indicating input mode ('*' for binary,
space for text), and name for each FILE.

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
For complete documentation, run: info coreutils 'md5sum invocation'
```
### Command Example (命令范例)
```
 md5sum

  Calculate MD5 cryptographic checksums.

  - Calculate the MD5 checksum for a file:
    md5sum filename1

  - Calculate MD5 checksums for multiple files:
    md5sum filename1 filename2

  - Read a file of MD5SUMs and verify all files have matching checksums:
    md5sum -c filename.md5
```
