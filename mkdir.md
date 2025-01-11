## MKDIR Command
Creates a directory.

## Syntax
```powershell
MKDIR [drive:]path
MD [drive:]path
```
If Command Extensions are enabled MKDIR changes as follows:

MKDIR creates any intermediate directories in the path, if needed.
For example, assume \a does not exist then:

    mkdir \a\b\c\d

is the same as:

    mkdir \a
    chdir \a
    mkdir b
    chdir b
    mkdir c
    chdir c
    mkdir d

which is what you would have to type if extensions were disabled.

## Examples
1. Creates the "test" directory in the current directory.
```powershell
mkdir test
```

2. Create a directory called "my directory" in the current directory. If you want a space in your directory name, it must be surrounded in quotes.
```powershell
mkdir "my directory"
```

3. Create the "test" directory with a specific path. This example creates the "test" directory in the c:\ directory.
```powershell
mkdir c:\test
```

4. Create the "test1" directory (if it does not already exist), and then the "test2" subdirectory, in the c:\ directory.
```powershell
mkdir c:\test1\test2
```
