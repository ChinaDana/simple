<sub>namespace com.google.devtools.simple.runtime</sub>
# Arrays #

Various array related runtime functions.

[Filter](ReferenceLibraryArrays#Filter.md)
> Filters the contents of an array.
[Join](ReferenceLibraryArrays#Join.md)
> Appends array elements to a become a single string.
[Split](ReferenceLibraryArrays#Split.md)
> Splits up the given string where a separator is being found.
[UBound](ReferenceLibraryArrays#UBound.md)
> Return the size of an array dimension.

---

### Filter ###

```
Static Function Filter(array As String(), str As String, include As Boolean) As String()
```

> Filters the contents of an array.

> Parameters:
> > array - array to search in
> > str - substring to search for in the array
> > include - if true then include matching strings in the result, otherwise exclude them

> Returns:
> > array containing (non-)matching array entries

---

### Join ###

```
Static Function Join(array As String(), separator As String) As String
```


> Appends array elements to a become a single string.

> Parameters:
> > array - array containing strings to be appended
> > separator - string append between array elements

> Returns:
> > string containing appended array elements

---

### Split ###

```
Static Function Split(str As String, separator As String, count As Integer) As String()
```


> Splits up the given string where a separator is being found.

> Parameters:
> > str - string to be split up
> > separator - separator to look for
> > count - number of times

> Returns:
> > array containing split string

---

### UBound ###

```
Static Function UBound(array As Variant, dim As Integer) As Integer
```


> Return the size of an array dimension.

> Parameters:
> > array - array whose size is requested
> > dim - dimension (1 for the first dimension, and so on)

> Returns:
> > size of the array dimension