## RMDIR Command
Removes (deletes) a directory.

## Syntax
```batchfile
RMDIR [/S] [/Q] [drive:]path
RD [/S] [/Q] [drive:]path

    /S      Removes all directories and files in the specified directory
            in addition to the directory itself.  Used to remove a directory
            tree.

    /Q      Quiet mode, do not ask if ok to remove a directory tree with /S
```

## Examples
**1. Remove the test directory, if it's empty.**
```batchfile
rmdir c:\test
```

**2. Permanently delete the test directory, subdirectories, and files.**
```batchfile
rmdir c:\test /s
```
> [!NOTE]
> Windows 2000, Windows XP and later versions of Windows can use this option with a prompt to permanently delete the test directory, subdirectories, and files. Adding the /q switch would suppress the prompt.
