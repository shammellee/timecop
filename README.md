[modeline]: # ( vim: set nospell: )

Rename files to a timestamp starting from now.


# Usage

```sh
$ timecop < <file_list>
```

Example:

```
$ timecop < my_files.txt
```

Where `my_files.txt` contains a list of newline-separated files:

```
foo.txt
bar.txt
baz.txt
qux.txt
quux.txt
```

The files specified in `my_files.txt` will be renamed like the following:

```
foo.txt  ➠  20190526_120210.txt
bar.txt  ➠  20190526_120211.txt
baz.txt  ➠  20190526_120212.txt
qux.txt  ➠  20190526_120213.txt
quux.txt ➠  20190526_120214.txt
```


# Caveats:

Subdirectories are not _yet_ supported; the command must be run in the same
directory as the files you wish to rename.

