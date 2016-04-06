<sub>namespace com.google.devtools.simple.runtime.components</sub>
# Panel #

A panel is a container for other components including other nested panels.

#### Events ####

[Initialize](ReferenceComponentPanel#Initialize.md)
> Initialization event.

#### Properties ####

[BackgroundColor](ReferenceComponentPanel#BackgroundColor.md)
> Property for controlling the component's background color.
[Column](ReferenceComponentPanel#Column.md)
> Property for controlling the column position when using a table layout.
[Height](ReferenceComponentPanel#Height.md)
> Property for controlling the component's height.
[Row](ReferenceComponentPanel#Row.md)
> Property for controlling the row position when using a table layout.
[Width](ReferenceComponentPanel#Width.md)
> Property for controlling the component's width.
[Layout](ReferenceComponentPanel#Layout.md)
> Property for controlling the component's layout.


---

### Initialize ###

```
Event Initialize()
```

> Event raised upon component initialization.

---

### BackgroundColor ###

```
Property BackgroundColor As Integer
```

> Reading from the BackgroundColor property returns the current background color of the component. The color value is encoded as _&Haarrggbb_ where _aa_ represents the alpha value (&H00 - transparent to &HFF - opaque), _rr_ represents the red, _gg_ the green and _bb_ the blue component of the color. Writing to the BackgroundColor property will set the background color of the component.

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

### Layout ###

```
Property Layout As Variant
```

> Reading from the Layout property returns the current layout object instance. For more information about layouts see LinearLayout, TableLayout and FrameLayout. Writing to the Layout property changes the layout to a different layout. The following predefined constants can be used: `Component.LAYOUT_LINEAR`, `Component.LAYOUT_TABLE` or `Component.LAYOUT_FRAME`.

> Note that once components have been added to the panel its layout cannot be changed any longer!