<sub>namespace com.google.devtools.simple.runtime</sub>
# Log #

Logging related runtime functions.

[Error](ReferenceLibraryLog#Error.md)
> Logs an error message.
[Info](ReferenceLibraryLog#Info.md)
> Logs an info message.
[Warning](ReferenceLibraryLog#Warning.md)
> Logs an warning message.

---

### Error ###

```
Static Sub Error(moduleName As String, message As String)
```

> Logs an error message.

> Parameters:
> > moduleName - name of the module reporting the message (e.g. "Simple Runtime Library")
> > message - text to log

---

### Warning ###

```
Static Sub Warning(moduleName As String, message As String)
```


> Logs an warning message.

> Parameters:
> > moduleName - name of the module reporting the message (e.g. "Simple Runtime Library")
> > message - text to log

---

### Info ###

```
Static Sub Info(moduleName As String, message As String)
```


> Logs an info message.

> Parameters:
> > moduleName - name of the module reporting the message (e.g. "Simple Runtime Library")
> > message - text to log