<sub>namespace com.google.devtools.simple.runtime.components</sub>
# TextBox #

Editable text box.

#### Events ####

[Initialize](ReferenceComponentTextBox#Initialize.md)
> Initialization event.
[GotFocus](ReferenceComponentTextBox#GotFocus.md)
> > Focus received event.
[LostFocus](ReferenceComponentTextBox#LostFocus.md)
> > Focus lost event.
[Validate](ReferenceComponentTextBox#Validate.md)
> > Input validation event.

#### Properties ####

[BackgroundColor](ReferenceComponentTextBox#BackgroundColor.md)

> Property for controlling the component's background color.
[Column](ReferenceComponentTextBox#Column.md)
> Property for controlling the column position when using a table layout.
[Height](ReferenceComponentTextBox#Height.md)
> Property for controlling the component's height.
[Row](ReferenceComponentTextBox#Row.md)
> Property for controlling the row position when using a table layout.
[Width](ReferenceComponentTextBox#Width.md)
> Property for controlling the component's width.
[FontBold](ReferenceComponentTextBox#FontBold.md)
> Property for controlling the component's font weight.
[FontItalic](ReferenceComponentTextBox#FontItalic.md)
> Property for controlling the component's font style.
[FontSize](ReferenceComponentTextBox#FontSize.md)
> Property for controlling the component's font size.
[FontTypeface](ReferenceComponentTextBox#FontTypeface.md)
> Property for controlling the component's font typeface.
[Justification](ReferenceComponentTextBox#Justification.md)
> Property for controlling the component's text justification.
[Text](ReferenceComponentTextBox#Text.md)
> Property for controlling the component's text.
[TextColor](ReferenceComponentTextBox#TextColor.md)
> Property for controlling the component's text color.
[Enabled](ReferenceComponentTextBox#Enabled.md)
> Property for controlling whether the component is enabled.
[Hint](ReferenceComponentTextBox#Hint.md)
> Property for controlling display of a hint.


---

### Initialize ###

```
Event Initialize()
```

> Event raised upon component initialization.

---

### GotFocus ###

```
Event GotFocus()
```

> Event raised after the component gains focus.

---

### LostFocus ###

```
Event LostFocus()
```

> Event raised after the component lost focus.

---

### Validate ###

```
Event Validate(text As String, ByRef accept As Boolean)
```

> Event raised after each character input. A handler for this event may check the input text and validate the input by setting the `accept` reference parameter.

> Parameters:
> > text - proposed content for textbox
> > accept - indicates whether to accept the input (default value is `True`)


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
### FontBold ###

```
Property FontBold As Boolean
```

> Reading from this property indicates the font weight. A value of `True` means that the component font is bold, `False` means normal. Writing to this property changes the changes the font weight.

> The default value of this property is `False`.

---

### FontItalic ###

```
Property FontItalic As Boolean
```

> Reading from this property indicates the font style. A value of `True` means that the component font is italic, `False` means normal. Writing to this property changes the changes the font style.

> The default value of this property is `False`.

---

### FontSize ###

```
Property FontSize As Single
```

> Reading from this property returns the font height in points. Writing to this property changes the changes the font height.

> The default value of this property is 14 points.

---

### FontTypeface ###

```
Property FontTypeface As Integer
```

> Reading from this property returns the font typeface. The value must be one of `Component.TYPEFACE_DEFAULT`, `Component.TYPEFACE_SERIF`, `Component.TYPEFACE_SANSSERIF` or `Component.TYPEFACE_MONOSPACE`. Writing to this property changes the changes the font typeface.

> The default value of this property is `Component.TYPEFACE_DEFAULT `.

---

### Justification ###

```
Property Justification As Integer
```

> Reading from this property returns the text justification. The value must be one of `Component.JUSTIFY_LEFT`, `Component.JUSTIFY_CENTER` or `Component.JUSTIFY_RIGHT`. Writing to this property changes the changes the text justification.

> The default value of this property is `Component.JUSTIFY_LEFT`.

---

### Text ###

```
Property Text As String
```

> Reading from this property returns the text displayed by the component. Writing to this property changes the changes the text displayed.

---

### TextColor ###

```
Property TextColor As Integer
```

> Reading from the TextColor property returns the current color of the text displayed by this component. The color value is encoded as _&Haarrggbb_ where _aa_ represents the alpha value (&H00 - transparent to &HFF - opaque), _rr_ represents the red, _gg_ the green and _bb_ the blue component of the color. Writing to the TextColor property will set the color for the text of the component.

> There are a number of predefined color constants: `Component.COLOR_NONE`, `Component.COLOR_BLACK`, `Component.COLOR_BLUE`, `Component.COLOR_CYAN`, `Component.COLOR_DKGRAY`, `Component.COLOR_GRAY`, `Component.COLOR_GREEN`, `Component.COLOR_LTGRAY`, `Component.COLOR_MAGENTA`, `Component.COLOR_RED`, `Component.COLOR_WHITE` and `Component.COLOR_YELLOW`.

---

### Enabled ###

```
Property Enabled As Boolean
```

> Reading from the Enabled property indicates whether the textbox is enabled. Writing to the Enabled property will enabled or disable the textbox.

> Textboxes are enabled by default.

---

### Hint ###

```
Property Hint As String
```

> Reading from the Hint property returns the text of the hint that will be shown for the textbox. Writing to the Hint property will change the hint being shown for the textbox.