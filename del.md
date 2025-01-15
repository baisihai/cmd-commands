## DEL Command
Delete files.

## Syntax
```powershell
DEL [/P] [/F] [/S] [/Q] [/A[[:]attributes]] names
ERASE [/P] [/F] [/S] [/Q] [/A[[:]attributes]] names

  names         Specifies a list of one or more files or directories.
                Wildcards may be used to delete multiple files. If a
                directory is specified, all files within the directory
                will be deleted.

  /P            Prompts for confirmation before deleting each file.
  /F            Force deleting of read-only files.
  /S            Delete specified files from all subdirectories.
  /Q            Quiet mode, do not ask if ok to delete on global wildcard
  /A            Selects files to delete based on attributes
  attributes    R  Read-only files            S  System files
                H  Hidden files               A  Files ready for archiving
                I  Not content indexed Files  L  Reparse Points
                O  Offline files              -  Prefix meaning not

If Command Extensions are enabled DEL and ERASE change as follows:

The display semantics of the /S switch are reversed in that it shows
you only the files that are deleted, not the ones it could not find.
```
> [!NOTE]
> Use the `rmdir` command to delete directories.

## Examples
**1. Delete a file from current directory.**
```powershell
del test.tmp
```

**2. Delete a file from specified path.**
```powershell
del c:\windows\test.tmp
```

**3. Delete multiple files from specified path.**
```powershell
del c:\windows\temp\*.*
```
