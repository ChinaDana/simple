<sub>namespace com.google.devtools.simple.runtime</sub>
# Files #

Various file related runtime functions.

[Close](ReferenceLibraryFiles#Close.md)
> Closes a file previously opened.
[Delete](ReferenceLibraryFiles#Delete.md)
> Deletes a file.
[Eof](ReferenceLibraryFiles#Eof.md)
> Checks whether the current file position is at the end of the file.
[Exists](ReferenceLibraryFiles#Exists.md)
> Checks whether a file or directory exists.
[IsDirectory](ReferenceLibraryFiles#IsDirectory.md)
> Checks whether the given name is the name of an existing directory.
[Mkdir](ReferenceLibraryFiles#Mkdir.md)
> Creates a new directory.
[Open](ReferenceLibraryFiles#Open.md)
> Opens an existing file or creates a new file for reading or writing.
[ReadBoolean](ReferenceLibraryFiles#ReadBoolean.md)
> Reads a Boolean value from a file.
[ReadByte](ReferenceLibraryFiles#ReadByte.md)
> Reads a Byte value from a file.
[ReadDouble](ReferenceLibraryFiles#ReadDouble.md)
> Reads a Double value from a file.
[ReadInteger](ReferenceLibraryFiles#ReadInteger.md)
> Reads an Integer value from a file.
[ReadLong](ReferenceLibraryFiles#ReadLong.md)
> Reads a Long value from a file.
[ReadShort](ReferenceLibraryFiles#ReadShort.md)
> Reads a Short value from a file.
[ReadSingle](ReferenceLibraryFiles#ReadSingle.md)
> Reads a Single value from a file.
[ReadString](ReferenceLibraryFiles#ReadString.md)
> Reads a String value from a file.
[Rename](ReferenceLibraryFiles#Rename.md)
> Renames a file.
[Rmdir](ReferenceLibraryFiles#Rmdir.md)
> Deletes a directory.
[Seek](ReferenceLibraryFiles#Seek.md)
> Positions the file pointer to an absolute position.
[Size](ReferenceLibraryFiles#Size.md)
> Returns the size of a file.
[WriteBoolean](ReferenceLibraryFiles#WriteBoolean.md)
> Writes a Boolean value to a file.
[WriteByte](ReferenceLibraryFiles#WriteByte.md)
> Writes a Byte value to a file.
[WriteDouble](ReferenceLibraryFiles#WriteDouble.md)
> Writes a Double value to a file.
[WriteInteger](ReferenceLibraryFiles#WriteInteger.md)
> Writes an Integer boolean value to a file.
[WriteLong](ReferenceLibraryFiles#WriteLong.md)
> Writes a Long value to a file.
[WriteShort](ReferenceLibraryFiles#WriteShort.md)
> Writes a Short value to a file.
[WriteSingle](ReferenceLibraryFiles#WriteSingle.md)
> Writes a Single value to a file.
[WriteString](ReferenceLibraryFiles#WriteString.md)
> Writes a String to a file.


---

### Rename ###

```
Static Sub Rename(oldname As String, newname As String)
```

> Renames a file. Causes a runtime error if the file doesn't exist.

> Parameters:
> > oldname - file name before renaming
> > newname - file name after renaming

---

### Delete ###

```
Static Sub Delete(name As String)
```


> Deletes a file.

> Parameters:
> > name - name of file to delete

---

### Mkdir ###

```
Static Sub Mkdir(name As String)
```


> Creates a new directory.

> Parameters:
> > name - name of new directory

---

### Rmdir ###

```
Static Sub Rmdir(name As String)
```


> Deletes a directory.

> Parameters:
> > name - name of directory to delete

---

### IsDirectory ###

```
Static Function IsDirectory(name As String) As Boolean
```


> Checks whether the given name is the name of an existing directory. Causes a runtime error if the directory doesn't exist.

> Parameters:
> > name - name to check

> Returns:
> > true if the name belongs to an existing directory, false otherwise

---

### Exists ###

```
Static Function Exists(name As String) As Boolean
```


> Checks whether a file or directory exists.

> Parameters:
> > name - file to check

> Returns:
> > true if the file or directory exists, false otherwise

---

### Open ###

```
Static Function Open(name As String) As Integer
```


> Opens an existing file or creates a new file for reading or writing.

> Parameters:
> > name - name of file to open or create

> Returns:
> > file handle

---

### Close ###

```
Static Sub Close(handle As Integer)
```


> Closes a file previously opened.

> Parameters:
> > handle - handle of file to close

---

### Eof ###

```
Static Function Eof(handle As Integer) As Boolean
```


> Checks whether the current file position is at the end of the file.

> Parameters:
> > handle - handle of file to check

> Returns:
> > true if the end of the file was reaches, false otherwise

---

### Seek ###

```
Static Function Seek(handle As Integer, offset As Long) As Long
```


> Positions the file pointer to an absolute position.

> Parameters:
> > handle - handle of file
> > offset - absolute position within file

> Returns:
> > new position within file

---

### Size ###

```
Static Function Size(handle As Integer) As Long
```


> Returns the size of a file.

> Parameters:
> > handle - handle of file

> Returns:
> > file size

---

### WriteString ###

```
Static Sub WriteString(handle As Integer, value As String)
```


> Writes a String to a file.

> Parameters:
> > handle - handle of file
> > value - value to write

---

### ReadString ###

```
Static Function ReadString(handle As Integer) As String
```


> Reads a String value from a file.

> Parameters:
> > handle - handle of file

> Returns:
> > value read

---

### WriteBoolean ###

```
Static Sub WriteBoolean(handle As Integer, value As Boolean)
```


> Writes a Boolean value to a file.

> Parameters:
> > handle - handle of file
> > value - value to write

---

### ReadBoolean ###

```
Static Function ReadBoolean(handle As Integer) As Boolean
```


> Reads a Boolean value from a file.

> Parameters:
> > handle - handle of file

> Returns:
> > value read

---

### WriteByte ###

```
Static Sub WriteByte(handle As Integer, value As Byte)
```


> Writes a Byte value to a file.

> Parameters:
> > handle - handle of file
> > value - value to write

---

### ReadByte ###

```
Static Function ReadByte(handle As Integer) As Byte
```


> Reads a Byte value from a file.

> Parameters:
> > handle - handle of file

> Returns:
> > value read

---

### WriteShort ###

```
Static Sub WriteShort(handle As Integer, value As Short)
```


> Writes a Short value to a file.

> Parameters:
> > handle - handle of file
> > value - value to write

---

### ReadShort ###

```
Static Function ReadShort(handle As Integer) As Short
```


> Reads a Short value from a file.

> Parameters:
> > handle - handle of file

> Returns:
> > value read

---

### WriteInteger ###

```
Static Sub WriteInteger(handle As Integer, value As Integer)
```


> Writes an Integer boolean value to a file.

> Parameters:
> > handle - handle of file
> > value - value to write

---

### ReadInteger ###

```
Static Function ReadInteger(handle As Integer) As Integer
```


> Reads an Integer value from a file.

> Parameters:
> > handle - handle of file

> Returns:
> > value read

---

### WriteLong ###

```
Static Sub WriteLong(handle As Integer, value As Long)
```


> Writes a Long value to a file.

> Parameters:
> > handle - handle of file
> > value - value to write

---

### ReadLong ###

```
Static Function ReadLong(handle As Integer) As Long
```


> Reads a Long value from a file.

> Parameters:
> > handle - handle of file

> Returns:
> > value read

---

### WriteSingle ###

```
Static Sub WriteSingle(handle As Integer, value As Single)
```


> Writes a Single value to a file.

> Parameters:
> > handle - handle of file
> > value - value to write

---

### ReadSingle ###

```
Static Function ReadSingle(handle As Integer) As Single
```


> Reads a Single value from a file.

> Parameters:
> > handle - handle of file

> Returns:
> > value read

---

### WriteDouble ###

```
Static Sub WriteDouble(handle As Integer, value As Double)
```


> Writes a Double value to a file.

> Parameters:
> > handle - handle of file
> > value - value to write

---

### ReadDouble ###

```
Static Function ReadDouble(handle As Integer) As Double
```


> Reads a Double value from a file.

> Parameters:
> > handle - handle of file

> Returns:
> > value read