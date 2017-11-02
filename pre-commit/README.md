# pre-commit

## Check file size

Default max file size = 1000000 bytes.

```console
$ cp check_file_size /path/to/repo/.git/hooks/pre-commit
$ mkdir -p foo/bar
$ mkfile 1000001 foo/bar/testfile
$ git add foo/bar/testfile
$ git commit
# Too large files

1000001 foo/bar/testfile
```
