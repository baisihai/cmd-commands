## RENAME Command
The `rename` command is used to rename a file or files from the Command Prompt.

`rename` and `ren` commands can be used interchangeably. They're the same.

## Syntax
```powershell
RENAME [drive:][path]filename1 filename2.
```
```powershell
REN [drive:][path]filename1 filename2.
```
Note that you cannot specify a new drive or path for your destination file.

## Examples
1. Rename file in the same folder 
```powershell
rename ABCDold.txt ABCDnew.txt
```

2. Rename file in specified folder
```powershell
rename c:\temp\ABCDold.txt ABCDnew.txt
```

3. Rename file extension and name
```powershell
rename ABCDold.bak ABCDnew.txt
```

4. Rename folder
```powershell
rename oldfolder "New Folder"
```

5. Rename multiple files  
```powershell
for %a in (*.*) do rename "%a" "ABCD%a"
```

6. Rename multiple files by file extensions
```powershell
for %a in (*.ipynb) do rename "%a" "ABCD%a"
```

7. Remove prefix from file names
For example to remove a prefix ABCD from ABCD1.txt, ABCD2.txt, ABCD3.txt etc. in order to get 1.txt, 2.txt, 3.txt, then simply use
```powershell
rename "ABCD*.mp4" "////*"
```
Note: You need the same number of / as the number of initial characters you would like to remove.
