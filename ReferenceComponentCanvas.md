<sub>namespace com.google.devtools.simple.runtime.components</sub>
# Canvas #

The Canvas component supplies a surface to draw on.

#### Events ####

[Initialize](ReferenceComponentCanvas#Initialize.md)
> Initialization event.
[Touched](ReferenceComponentCanvas#Touched.md)
> Touch event.

#### Properties ####

[BackgroundColor](ReferenceComponentCanvas#BackgroundColor.md)
> Property for controlling the component's background color.
[Column](ReferenceComponentCanvas#Column.md)
> Property for controlling the column position when using a table layout.
[Height](ReferenceComponentCanvas#Height.md)
> Property for controlling the component's height.
[Row](ReferenceComponentCanvas#Row.md)
> Property for controlling the row position when using a table layout.
[Width](ReferenceComponentCanvas#Width.md)
> Property for controlling the component's width.
[BackgroundImage](ReferenceComponentCanvas#BackgroundImage.md)
> Property for controlling the background image of the canvas.
[PaintColor](ReferenceComponentCanvas#PaintColor.md)
> Property for controlling the paint color.

#### Functions ####
[Clear](ReferenceComponentCanvas#Clear.md)
> Clears the canvas.
[DrawCircle](ReferenceComponentCanvas#DrawCircle.md)
> Draws a circle at the given coordinates on the canvas, with the given radius
[DrawLine](ReferenceComponentCanvas#DrawLine.md)
> Draws a line between the given coordinates on the canvas.
[DrawPoint](ReferenceComponentCanvas#DrawPoint.md)
> Draws a point at the given coordinates on the canvas.


---

### Initialize ###

```
Event Initialize()
```

> Event raised upon component initialization.

---

### Touched ###

```
Event Touched(x As Integer, y As Integer)
```

> Event raised when the device screen is touched.

---

### BackgroundColor ###

```
Property BackgroundColor As Integer
```

> Reading from the BackgroundColor property returns the current background color of the component. The color value is encoded as _&Haarrggbb_ where _aa_ represents the alpha value (&H00 - transparent to &HFF - opaque), _rr_ represents the red, _gg_ the green and _bb_ the blue component of the color. Writing to the BackgroundColor property will set the background color of the component. The default background color of the Canvas component is `Component.COLOR_WHITE`.

> There are a number of predefined color constants: `Component.COLOR_NONE`, `Component.COLOR_BLACK`, `Component.COLOR_BLUE`, `Component.COLOR_CYAN`, `Component.COLOR_DKGRAY`, `Component.COLOR_GRAY`, `Component.COLOR_GREEN`, `Component.COLOR_LTGRAY`, `Component.COLOR_MAGENTA`, `Component.COLOR_RED`, `Component.COLOR_WHITE` and `Component.COLOR_YELLOW`.

---

### Column ###

```
Property Column As Integer
```

> Reading from the Column property returns the current column position within a table layout. Writing to the Column property will set the column position of the component within a table layout. This property has no meaning for any other layout.

---

### Height ###

```
Property Height As Integer
```

> Reading from the Height property returns the current height of the component in pixels. Writing to the Height property changes the height of the component to the given value in pixels. There are two special values. `Component.LENGTH_PREFERRED` sets the preferred height of the component which depends on the contents of the component. `Component.LENGTH_FILL_PARENT` sets the height of the component to its maximum to fill the height of its parent container.

---

### Row ###

```
Property Row As Integer
```

> Reading from the Row property returns the current row position within a table layout. Writing to the Row property will set the row position of the component within a table layout. This property has no meaning for any other layout.

---

### Width ###

```
Property Width As Integer
```

> Reading from the Width property returns the current width of the component in pixels. Writing to the Width property changes the width of the component to the given value in pixels. There are two special values. `Component.LENGTH_PREFERRED` sets the preferred width of the component which depends on the contents of the component. `Component.LENGTH_FILL_PARENT` sets the width of the component to its maximum to fill the width of its parent container.

---

### BackgroundImage ###

```
Property BackgroundImage As String
```

> Writing to this property changes the background image shown on the component. The value assigned to this property should be the name of a file in the project's assets directory. This property is write-only.

---

### Clear ###

```
Sub Clear()
```

> Clears the canvas (fills it with the background color).

---

### DrawPoint ###

```
Sub DrawPoint(x As Integer, y As Integer)
```

> Draws a point at the given coordinates on the canvas.

> Parameters:
> > x - x coordinate<br>
<blockquote>y - y coordinate<br>
<hr />
<h3>DrawCircle</h3></blockquote></li></ul>

<pre><code>Sub DrawCircle(x As Integer, y As Integer, r As Single)<br>
</code></pre>

<blockquote>Draws a circle at the given coordinates on the canvas, with the given radius


> Parameters:
> > x - x coordinate<br>
<blockquote>y - y coordinate<br>
r - radius<br>
<hr />
<h3>DrawLine</h3></blockquote></blockquote>

<pre><code>Sub DrawLine(x1 As Integer, y1 As Integer, x2 As Integer, y2 As Integer)<br>
</code></pre>

<blockquote>Draws a line between the given coordinates on the canvas.</blockquote>

<blockquote>Parameters:<br>
<blockquote>x1 - x coordinate of first point<br>
y1 - y coordinate of first point<br>
x2 - x coordinate of second point<br>
y2 - y coordinate of second point