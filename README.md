# OpenAny
A bash script used to open a type-arbitrary file on Linux.

## License
[The MIT License](http://tchel.mit-license.org)

## Usage

You can get help information as follows:

```shell
[user@A ~]$ opan -h

Usage:  opan [-h] | [ file [options] ]
  [-h     ]: print this help information.
  [file   ]: name of the file to open.
  [options]: options to pass to the invoked file-open tool.
```

If you want to open any file, just run `$ opan filename`, __opan__ will automatically detect file type according to file extension, and select a binding tool to open the file _filename_.

So far, __opan__ supports:

| file extension                      | invoked tool |
| ----------------------------------- | ------------ |
| .txt, .log, .conf, .dat, .inc, .cpt | vim          |
| .c, .cpp, .h                        | vim          |
| .f, .for, .f90, .F, .FOR, .F90      | vim          |
| .cu                                 | vim          |
| .m, .py                             | vim          |
| .sh, .bat                           | vim          |
| .tex, .sty, .bib                    | vim          |
| .pbs, .lsf                          | vim          |
| .json                               | vim          |
| .yml                                | vim          |
| .html                               | vim          |
| .pdf, .eps, .ps                     | evince       |
| .png, .jpg, .gif, .tif              | eog          |
| .tar, .tgz, .gz, .bz2               | tar          |
| .md                                 | typora       |
| .nc                                 | ncdump       |

## Author

Tche LIU, <seistche@gmail.com>, USTC

![OpenAny](./OpAn.png)
