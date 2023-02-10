# Scripts

## viman
viman is a simple script that opens man pages in vim for easier navigation.

### Example

```sh
$ viman man
```

```
1   MAN(1)                                                                             Manual pager utils                                                                             MAN(1) 
  1 
  2 NAME
  3        man - an interface to the system reference manuals
  4 
  5 SYNOPSIS
  6        man [man options] [[section] page ...] ...
  7        man -k [apropos options] regexp ...
  8        man -K [man options] [section] term ...
  9        man -f [whatis options] page ...
 10        man -l [man options] file ...
 11        man -w|-W [man options] page ...
 12 
 13 DESCRIPTION
 14        man  is  the system's manual pager.  Each page argument given to man is normally the name of a program, utility or function.  The manual page associated with each of these argu‐
 15        ments is then found and displayed.  A section, if provided, will direct man to look only in that section of the manual.  The default action is to search in all of the  available
 16        sections following a pre-defined order (see DEFAULTS), and to show only the first page found, even if page exists in several sections.
 17 
 18        The table below shows the section numbers of the manual followed by the types of pages they contain.
 19 
 20        1   Executable programs or shell commands
 21        2   System calls (functions provided by the kernel)
 22        3   Library calls (functions within program libraries)
 23        4   Special files (usually found in /dev)
 24        5   File formats and conventions, e.g. /etc/passwd
 25        6   Games
 26        7   Miscellaneous (including macro packages and conventions), e.g. man(7), groff(7), man-pages(7)
 27        8   System administration commands (usually only for root)
 28        9   Kernel routines [Non standard]
 29 
 30        A manual page consists of several sections.
                                                          .
                                                          .
                                                          .
```

## cloc-git
cloc-git displays the line count for each language used in a git repository.

### Example 

```
cloc-git example  
```
```
11:58:19 PM
Cloning into 'temp-linecount-repo'...
warning: --depth is ignored in local clones; use file:// instead.
done.
Updating files: 100% (12056/12056), done.
('temp-linecount-repo' will be deleted automatically)


   11561 text files.
    9459 unique files.                                          
    2560 files ignored.

1 error:
Line count, exceeded timeout:  temp-linecount-repo/frontend/node_modules/needle/lib/needle.js

github.com/AlDanial/cloc v 1.94  T=9.34 s (1012.4 files/s, 213884.3 lines/s)
---------------------------------------------------------------------------------------
Language                             files          blank        comment           code
---------------------------------------------------------------------------------------
JavaScript                            6879          48039         211591        1242259
Python                                 688          34627          47550         173999
TypeScript                            1138           8178          52097          71480
JSON                                   327              2              0          50415
Markdown                               287          14463              0          32559
CSS                                     26            621             35           4123
HTML                                    22            536             67           2126
Text                                    24            144              0           1550
Windows Module Definition                5             83              0            451
YAML                                    28             32              9            311
LESS                                    17             21              0            286
PHP                                      1             13             19            124
XML                                      7              0              1             98
Fish Shell                               1             18             14             68
SVG                                      2              0              1             68
PowerShell                               1             10              4             46
Bourne Again Shell                       2             11              1             43
C Shell                                  1             13              7             35
reStructuredText                         1              5              0             23
Nix                                      1              1              0             19
Bourne Shell                             1              4              0              8
---------------------------------------------------------------------------------------
SUM:                                  9459         106821         311396        1580091
---------------------------------------------------------------------------------------```

