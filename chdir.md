## CHDIR Command
Displays the name of or changes the current directory.

## Syntax
```powershell
CHDIR [/D] [drive:][path]
CHDIR [..]
CD [/D] [drive:][path]
CD [..]
```
..   Specifies that you want to change to the parent directory.

Type CD drive: to display the current directory in the specified drive.
Type CD without parameters to display the current drive and directory.

Use the /D switch to change current drive in addition to changing current
directory for a drive.

If Command Extensions are enabled CHDIR changes as follows:

The current directory string is converted to use the same case as
the on disk names.  So CD C:\TEMP would actually set the current
directory to C:\Temp if that is the case on disk.

CHDIR command does not treat spaces as delimiters, so it is possible to
CD into a subdirectory name that contains a space without surrounding
the name with quotes.  For example:

    cd \winnt\profiles\username\programs\start menu

is the same as:

    cd "\winnt\profiles\username\programs\start menu"

which is what you would have to type if extensions were disabled.

## Examples
1. Displays the current directory
```powershell
chdir
```

2. Change to the root directory of the drive.
```powershell
chdir \
```

3. Change to a specific directory. For example, if you are in the C:\temp> directory, this would take you to C:\Windows> directory.
```powershell
chdir c:\Windows
```

4. Change to a sub-directory. For example, if you are in the C:\temp> directory, this would take you to C:\Temp\SubFolder> directory.
```powershell
chdir SubFolder
```

5. Goes back one directory. For example, if you are in the C:\Temp\SubFolder> directory, this would take you to C:\Temp> directory.
```powershell
chdir ..
```
