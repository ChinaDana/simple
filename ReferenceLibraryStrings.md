<sub>namespace com.google.devtools.simple.runtime</sub>
# Strings #

Various string related runtime functions.

[InStr](ReferenceLibraryStrings#InStr.md)
> Searches for a string in another string.
[InStrRev](ReferenceLibraryStrings#InStrRev.md)
> Searches for a string in another string starting at the end of that string.
[LCase](ReferenceLibraryStrings#LCase.md)
> Converts the given string to all lowercase.
[Left](ReferenceLibraryStrings#Left.md)
> Returns the specified number of characters from the start of the given string.
[Len](ReferenceLibraryStrings#Len.md)
> Returns the number of characters in the given string.
[LTrim](ReferenceLibraryStrings#LTrim.md)
> Removes leading space characters from the given string.
[Mid](ReferenceLibraryStrings#Mid.md)
> Returns the specified number of characters from the given string starting from the given index.
[Replace](ReferenceLibraryStrings#Replace.md)
> Replaces occurrences of one string with another string in the given string.
[Right](ReferenceLibraryStrings#Right.md)
> Returns the specified number of characters from the end of the given string.
[RTrim](ReferenceLibraryStrings#RTrim.md)
> Removes trailing space characters from the given string.
[StrComp](ReferenceLibraryStrings#StrComp.md)
> Compares the two given strings lexicographically.
[StrReverse](ReferenceLibraryStrings#StrReverse.md)
> Reverses the given string.
[Trim](ReferenceLibraryStrings#Trim.md)
> Removes leading and trailing space characters from the given string.
[UCase](ReferenceLibraryStrings#UCase.md)
> Converts the given string to all uppercase.


---

### InStr ###

```
Static Function InStr(str1 As String, str2 As String, start As Integer) As Integer
```

> Searches for a string in another string.

> Parameters:
> > str1 - string to search in
> > str2 - string to search for
> > start - search start index within str1

> Returns:
> > index at which str2 was found within str1 or a negative value if str2 was not found within str1

---

### InStrRev ###

```
Static Function InStrRev(str1 As String, str2 As String, start As Integer) As Integer
```


> Searches for a string in another string starting at the end of that string.

> Parameters:
> > str1 - string to search in
> > str2 - string to search for
> > start - search start index within str1

> Returns:
> > index at which str2 was found within str1 or a negative value if str2 was not found within str1

---

### LCase ###

```
Static Sub LCase(ByRef str As String)
```


> Converts the given string to all lowercase.

> Parameters:
> > str - string to convert to lowercase

---

### UCase ###

```
Static Sub  UCase(ByRef str As String)
```


> Converts the given string to all uppercase.

> Parameters:
> > str - string to convert to uppercase

---

### Left ###

```
Static Function Left(str As String, len As Integer) As String
```


> Returns the specified number of characters from the start of the given string.

> Parameters:
> > str - string to return characters from
> > len - number of characters to return

> Returns:
> > substring of the given string

---

### Right ###

```
Static Function Right(str As String, len As Integer) As String
```


> Returns the specified number of characters from the end of the given string.

> Parameters:
> > str - string to return characters from
> > len - number of characters to return

> Returns:
> > substring of the given string

---

### Mid ###

```
Static Function Mid(str As String, start As Integer, len As Integer) As String
```


> Returns the specified number of characters from the given string starting from the given index.

> Parameters:
> > str - string to return characters from
> > start - start index within str
> > len - number of characters to return

> Returns:
> > substring of the given string

---

### Len ###

```
Static Function Len(str As String) As Integer
```


> Returns the number of characters in the given string.

> Parameters:
> > str - string to get length of

> Returns:
> > number of characters (length) of the given string

---

### Trim ###

```
Static Sub Trim(ByRef str As String)
```


> Removes leading and trailing space characters from the given string.

> Parameters:
> > str - string to trim

---

### LTrim ###

```
Static Sub LTrim(ByRef str As String)
```


> Removes leading space characters from the given string.

> Parameters:
> > str - string to trim

---

### RTrim ###

```
Static Sub RTrim(ByRef str As String)
```


> Removes trailing space characters from the given string.

> Parameters:
> > str - string to trim

---

### Replace ###

```
Static Sub Replace(ByRef str As String, find As String,  replace As String, start As Integer, count As Integer)
```


> Replaces occurrences of one string with another string in the given string.

> Parameters:
> > str - string to modify
> > find - string to find
> > replace - string to replace found string with
> > start - start index within str
> > count - number of times to perform the replacement (-1 to replace all occurrences)

---

### StrComp ###

```
Static Function StrComp(str1 As String, str2 As String) As Integer
```


> Compares the two given strings lexicographically.

> Parameters:
> > str1 - first string of comparison
> > str2 - second string of comparison

> Returns:
> > 0 if the strings are equal, a negative number if str2 follows str1 and a positive number if str1 follows str2

---

### StrReverse ###

```
Static Sub StrReverse(ByRef str As String)
```


> Reverses the given string.

> Parameters:
> > str - string to reverse