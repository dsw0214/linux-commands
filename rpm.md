# Linux rpm Command
### Command Introduction (命令介绍)
-------------------
> ** rpm - RPM Package Manager **
   
### Command Format and Options (命令格式和选项)
```
#rpm --help
Usage: rpm [OPTION...]

Query/Verify package selection options:
  -a, --all                        query/verify all packages
  -f, --file                       query/verify package(s) owning file
  -g, --group                      query/verify package(s) in group
  -p, --package                    query/verify a package file
  --pkgid                          query/verify package(s) with package
                                   identifier
  --hdrid                          query/verify package(s) with header
                                   identifier
  --triggeredby                    query the package(s) triggered by the
                                   package
  --whatrequires                   query/verify the package(s) which require a
                                   dependency
  --whatprovides                   query/verify the package(s) which provide a
                                   dependency
  --nomanifest                     do not process non-package files as
                                   manifests

Query options (with -q or --query):
  -c, --configfiles                list all configuration files
  -d, --docfiles                   list all documentation files
  -L, --licensefiles               list all license files
  --dump                           dump basic file information
  -l, --list                       list files in package
  --queryformat=QUERYFORMAT        use the following query format
  -s, --state                      display the states of the listed files

Verify options (with -V or --verify):
  --nofiledigest                   don't verify digest of files
  --nofiles                        don't verify files in package
  --nodeps                         don't verify package dependencies
  --noscript                       don't execute verify script(s)

Install/Upgrade/Erase options:
  --allfiles                       install all files, even configurations
                                   which might otherwise be skipped
  --allmatches                     remove all packages which match <package>
                                   (normally an error is generated if
                                   <package> specified multiple packages)
  --badreloc                       relocate files in non-relocatable package
  -e, --erase=<package>+           erase (uninstall) package
  --excludedocs                    do not install documentation
  --excludepath=<path>             skip files with leading component <path> 
  --force                          short hand for --replacepkgs --replacefiles
  -F, --freshen=<packagefile>+     upgrade package(s) if already installed
  -h, --hash                       print hash marks as package installs (good
                                   with -v)
  --ignorearch                     don't verify package architecture
  --ignoreos                       don't verify package operating system
  --ignoresize                     don't check disk space before installing
  -i, --install                    install package(s)
  --justdb                         update the database, but do not modify the
                                   filesystem
  --nodeps                         do not verify package dependencies
  --nofiledigest                   don't verify digest of files
  --nocontexts                     don't install file security contexts
  --noorder                        do not reorder package installation to
                                   satisfy dependencies
  --noscripts                      do not execute package scriptlet(s)
  --notriggers                     do not execute any scriptlet(s) triggered
                                   by this package
  --nocollections                  do not perform any collection actions
  --oldpackage                     upgrade to an old version of the package
                                   (--force on upgrades does this
                                   automatically)
  --percent                        print percentages as package installs
  --prefix=<dir>                   relocate the package to <dir>, if
                                   relocatable
  --relocate=<old>=<new>           relocate files from path <old> to <new>
  --replacefiles                   ignore file conflicts between packages
  --replacepkgs                    reinstall if the package is already present
  --test                           don't install, but tell if it would work or
                                   not
  -U, --upgrade=<packagefile>+     upgrade package(s)
  --reinstall=<packagefile>+       reinstall package(s)

Common options for all rpm modes and executables:
  -D, --define='MACRO EXPR'        define MACRO with value EXPR
  --undefine=MACRO                 undefine MACRO
  -E, --eval='EXPR'                print macro expansion of EXPR
  --macros=<FILE:...>              read <FILE:...> instead of default file(s)
  --noplugins                      don't enable any plugins
  --nodigest                       don't verify package digest(s)
  --nosignature                    don't verify package signature(s)
  --rcfile=<FILE:...>              read <FILE:...> instead of default file(s)
  -r, --root=ROOT                  use ROOT as top level directory (default:
                                   "/")
  --dbpath=DIRECTORY               use database in DIRECTORY
  --querytags                      display known query tags
  --showrc                         display final rpmrc and macro configuration
  --quiet                          provide less detailed output
  -v, --verbose                    provide more detailed output
  --version                        print the version of rpm being used

Options implemented via popt alias/exec:
  --scripts                        list install/erase scriptlets from
                                   package(s)
  --setperms                       set permissions of files in a package
  --setugids                       set user/group ownership of files in a
                                   package
  --conflicts                      list capabilities this package conflicts
                                   with
  --obsoletes                      list other packages removed by installing
                                   this package
  --provides                       list capabilities that this package provides
  --requires                       list capabilities required by package(s)
  --info                           list descriptive information from package(s)
  --changelog                      list change logs for this package
  --xml                            list metadata in xml
  --triggers                       list trigger scriptlets from package(s)
  --last                           list package(s) by install time, most
                                   recent first
  --dupes                          list duplicated packages
  --filesbypkg                     list all files from each package
  --fileclass                      list file names with classes
  --filecolor                      list file names with colors
  --fscontext                      list file names with security context from
                                   file system
  --fileprovide                    list file names with provides
  --filerequire                    list file names with requires
  --filecaps                       list file names with POSIX1.e capabilities

Help options:
  -?, --help                       Show this help message
  --usage                          Display brief usage message
```
### Command Example (命令范例)
-------------------
** RPM Package Manager. **

- Show version of httpd package:

  ` rpm -q httpd`

- List versions of all matching packages:

  ` rpm -qa 'mariadb*'`

- Identify owner of a file and show version of the package:

  ` rpm -qf /etc/postfix/main.cf`

- List package-owned files:

  ` rpm -ql kernel`

- Show scriptlets from an RPM file:

  ` rpm -qp --scripts some.rpm`

- Show changed, missing and/or incorrectly installed files of matching packages:

  ` rpm -Va 'php-*'`

