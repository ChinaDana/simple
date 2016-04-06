<sub>namespace com.google.devtools.simple.runtime</sub>
# Math #

Various mathematical runtime functions.

[E](ReferenceLibraryMath#E.md)
> Euler's constant.
[PI](ReferenceLibraryMath#PI.md)
> Pi.

[Abs](ReferenceLibraryMath#Abs.md)
> Returns the absolute value of the given value.
[Atn](ReferenceLibraryMath#Atn.md)
> Returns the arctangent for the given value.
[Atn2](ReferenceLibraryMath#Atn2.md)
> Returns the angle theta from the conversion of rectangular coordinates (x, y) to polar coordinates (r, theta>).
[Cos](ReferenceLibraryMath#Cos.md)
> Returns the cosine for the given value.
[DegreesToRadians](ReferenceLibraryMath#DegreesToRadians.md)
> Converts an angle measured in degrees to an approximation in radians.
[Exp](ReferenceLibraryMath#Exp.md)
> Returns e (euler's constant) raised to the power of the given value.
[Int](ReferenceLibraryMath#Int.md)
> Returns the integer part of the given number.
[Log](ReferenceLibraryMath#Log.md)
> Returns the natural logarithm for the given number.
[Max](ReferenceLibraryMath#Max.md)
> Returns the greater of two values.
[Min](ReferenceLibraryMath#Min.md)
> Returns the smaller of two values.
[RadiansToDegrees](ReferenceLibraryMath#RadiansToDegrees.md)
> Converts an angle measured in radians to an approximation in degrees.
[Rnd](ReferenceLibraryMath#Rnd.md)
> Returns a random number in the range between 0.0 (inclusive) and 1.0 (exclusive).
[Sgn](ReferenceLibraryMath#Sgn.md)
> Indicates the sign for the given value.
[Sin](ReferenceLibraryMath#Sin.md)
> Returns the sine for the given value.
[Sqr](ReferenceLibraryMath#Sqr.md)
> Returns the square root for the given value.
[Tan](ReferenceLibraryMath#Tan.md)
> Returns the tangent for the given value.


---

### E ###

```
Const E As Double
```

> Euler's constant.

---

### PI ###

```
Const PI As Double
```

> Pi.

---

### Abs ###

```
Static Function Abs(v As Variant) As Variant
```

> Returns the absolute value of the given value.

> Parameters:
> > v - value

> Returns:
> > absolute value

---

### Atn ###

```
Static Function Atn(v As Double) As Double
```


> Returns the arctangent for the given value.

> Parameters:
> > v - value

> Returns:
> > arctangent of v

---

### Atn2 ###

```
Static Function Atn2(y As Double, x As Double) As Double
```


> Returns the angle theta from the conversion of rectangular coordinates (x, y) to polar coordinates (r, theta>).

> Parameters:
> > y - the ordinate coordinate
> > x - the abscissa coordinate

> Returns:
> > the theta component of the point (r, theta) in polar coordinates that corresponds to the point (x, y) in Cartesian coordinates

---

### Cos ###

```
Static Function Cos(v As Double) As Double
```


> Returns the cosine for the given value.

> Parameters:
> > v - value

> Returns:
> > cosine of v

---

### Exp ###

```
Static Function Exp(v As Double) As Double
```


> Returns e (euler's constant) raised to the power of the given value.

> Parameters:
> > v - value

> Returns:
> > e to the power of v

---

### Int ###

```
Static Function Int(v As Variant) As Long
```


> Returns the integer part of the given number.

> Parameters:
> > v - value

> Returns:
> > integer part of v

---

### Log ###

```
Static Function Log(v As Double) As Double
```


> Returns the natural logarithm for the given number.

> Parameters:
> > v - value

> Returns:
> > natural logarithm for v

---

### Max ###

```
Static Function Max(v1 As Variant, v2 As Variant) As Variant
```


> Returns the greater of two values.

> Parameters:
> > v1 - first value
> > v2 - second value

> Returns:
> > greater value of v1 and v2

---

### Min ###

```
Static Function Min(v1 As Variant, v2 As Variant) As Variant
```


> Returns the smaller of two values.

> Parameters:
> > v1 - first value
> > v2 - second value

> Returns:
> > smaller value of v1 and v2

---

### Rnd ###

```
Static Function Rnd() As Double
```


> Returns a random number in the range between 0.0 (inclusive) and 1.0 (exclusive).

> Returns:
> > random number (between 0.0 and 1.0)

---

### Sin ###

```
Static Function Sin(v As Double) As Double
```


> Returns the sine for the given value.

> Parameters:
> > v - value

> Returns:
> > sine of v

---

### Sgn ###

```
Static Function Sgn(v As Double) As Integer
```


> Indicates the sign for the given value.

> Parameters:
> > v - value

> Returns:
    1. for positive values, 0 for zero, and -1 for negative values

---

### Sqr ###

```
Static Function Sqr(v As Double) As Double
```

> Returns the square root for the given value.

> Parameters:
> > v - value

> Returns:
> > square root of v

---

### Tan ###

```
Static Function Tan(v As Double) As Double
```


> Returns the tangent for the given value.

> Parameters:
> > v - value

> Returns:
> > tangent of v

---

### DegreesToRadians ###

```
Static Function DegreesToRadians(d As Double) As Double
```


> Converts an angle measured in degrees to an approximation in radians.

> Parameters:
> > d - value in degrees

> Returns:
> > radian approximation to d degrees

---

### RadiansToDegrees ###

```
Static Function RadiansToDegrees(r As Double) As Double
```


> Converts an angle measured in radians to an approximation in degrees.

> Parameters:
> > r - value in radians

> Returns:
> > degree approximation to r radians