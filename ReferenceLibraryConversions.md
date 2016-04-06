<sub>namespace com.google.devtools.simple.runtime</sub>
# Conversions #

Various conversion related runtime functions.

[Asc](ReferenceLibraryConversions#Asc.md)
> Returns the unicode value of the first character of the given string.
[Chr](ReferenceLibraryConversions#Chr.md)
> Returns a string for the given unicode value.
[Hex](ReferenceLibraryConversions#Hex.md)
> Returns a string containing the hexadecimal value for the given value.

---

### Asc ###

```
Static Function Asc(str As String) As Integer
```

> Returns the unicode value of the first character of the given string.

> Parameters:
> > str - string to convert first character of

> Returns:
> > unicode value of first character of str

---

### Chr ###

```
Static Function Chr(value As Integer) As String
```


> Returns a string for the given unicode value.

> Parameters:
> > value - unicode value to convert into a string

> Returns:
> > string consisting of given unicode value

---

### Hex ###

```
Static Function Hex(v As Variant) As String
```


> Returns a string containing the hexadecimal value for the given value. If the given value is not w whole number then its integer part will be used.

> Parameters:
> > v - value

> Returns:
> > string with hexadecimal value of v