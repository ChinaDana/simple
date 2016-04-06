<sub>namespace com.google.devtools.simple.runtime</sub>
# Assertions #

Assertions allow test against assumptions about the runtime state of an application. A failing assertion will result in an AssertionFailure runtime error.

[AssertFalse](ReferenceLibraryAssertions#AssertFalse.md)
> Tests whether an assertion is false.
[AssertTrue](ReferenceLibraryAssertions#AssertTrue.md)
> Tests whether an assertion is true.
> 
---

### AssertTrue ###

```
Static Sub AssertTrue(expression As Variant)
```

> Tests whether an assertion is true. Evaluates the given expression and causes an AssertionFailure runtime error if the expression does not evaluate to True.

> Parameters:
> > expression - expression to test

---

### AssertFalse ###

```
Static Sub AssertFalse(expression As Variant)
```


> Tests whether an assertion is false. Evaluates the given expression and causes an AssertionFailure runtime error if the expression does not evaluate to False.

> Parameters:
> > expression - expression to test