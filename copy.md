## COPY Command
Copies one or more files to another location.

## Syntax
```batchfile
COPY [/D] [/V] [/N] [/Y | /-Y] [/Z] [/L] [/A | /B ] source [/A | /B]
     [+ source [/A | /B] [+ ...]] [destination [/A | /B]]

  source       Specifies the file or files to be copied.
  /A           Indicates an ASCII text file.
  /B           Indicates a binary file.
  /D           Allow the destination file to be created decrypted
  destination  Specifies the directory and/or filename for the new file(s).
  /V           Verifies that new files are written correctly.
  /N           Uses short filename, if available, when copying a file with a
               non-8dot3 name.
  /Y           Suppresses prompting to confirm you want to overwrite an
               existing destination file.
  /-Y          Causes prompting to confirm you want to overwrite an
               existing destination file.
  /Z           Copies networked files in restartable mode.
  /L           If the source is a symbolic link, copy the link to the target
               instead of the actual file the source link points to.
```

The switch /Y may be preset in the COPYCMD environment variable.
This may be overridden with /-Y on the command line.  Default is
to prompt on overwrites unless COPY command is being executed from
within a batch script.

To append files, specify a single file for destination, but multiple files
for source (using wildcards or file1+file2+file3 format).

## Examples
**1. Copy the test.txt file to the temp directory; the test.txt can be substituted for any file(s).**
```batchfile
copy test.txt c:\temp
```

**2. Copy all .txt files to the temp directory.**
```batchfile
copy *.txt c:\temp
```

**3. Copy all files to the temp directory.**
```batchfile
copy *.* c:\temp
```

**4. Copy all files to the temp directory.**  
If the file already exists in the temp directory it would usually prompt to overwrite the file. Use the /y switch to suppress prompting to confirm you want to overwrite an existing destination file.

```batchfile
copy *.* c:\temp /y
```

**5. Copy the file "my file.txt" into the temp directory.**  
For file name or directory name with a space, it must be surrounded with quotes. 

```batchfile
copy "my file.txt" temp
```

**6. Copy the contents in test2.txt and combines it with the contents in test1.txt.**

```batchfile
copy test1.txt+test2.txt
```

**7. Create a test.txt file with console inputs.**  
Once the command is executed, type the text contents. Save and exit the file by pressing Ctrl+Z. However, it's easier to use a file editor to edit to view and edit files.

```batchfile
copy con test.txt
```
