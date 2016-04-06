<sub>namespace com.google.devtools.simple.runtime.components</sub>
# Form #

Form is the base object of all forms defined by applications. A form is the root container for all components on it.

#### Events ####

[Initialize](ReferenceComponentForm#Initialize.md)
> Initialization event.
[Keyboard](ReferenceComponentForm#Keyboard.md)
> Keyboard input event.
[MenuSelected](ReferenceComponentForm#MenuSelected.md)
> Menu selection event.
[TouchGesture](ReferenceComponentForm#TouchGesture.md)
> Touch gesture event.

#### Properties ####

[BackgroundColor](ReferenceComponentForm#BackgroundColor.md)
> Property for controlling the form's background color.
[Height](ReferenceComponentForm#Height.md)
> Property for reading the forms's height.
[Width](ReferenceComponentForm#Width.md)
> Property for reading the forms's width.
[BackgroundImage](ReferenceComponentForm#BackgroundImage.md)
> Property for controlling the form's background image.
[Layout](ReferenceComponentForm#Layout.md)
> Property for controlling the form's layout.
[Scrollable](ReferenceComponentForm#Scrollable.md)
> Property for controlling whether the content is scrollable.
[Title](ReferenceComponentForm#Title.md)
> Property for controlling the form's title.


---

### Initialize ###

```
Event Initialize()
```

> Event raised upon form initialization. Inside of an event handler for this event is the best place for adding components dynamically to a form. For more information of dynamic forms see [How To Write A Simple Application](HowToWriteASimpleApplication#Static_Forms_vs._Dynamic_Forms.md).


---

### Keyboard ###

```
Event Keyboard(keycode As Integer)
```

> Event raised after keyboard input.

> Parameters:
> > keycode - constant identifying pressed key (one of `Component.KEYCODE_0`, `Component.KEYCODE_1`, `Component.KEYCODE_2`, `Component.KEYCODE_3`, `Component.KEYCODE_4`, `Component.KEYCODE_5`, `Component.KEYCODE_6`, `Component.KEYCODE_7`, `Component.KEYCODE_8`, `Component.KEYCODE_9`, `Component.KEYCODE_A`, `Component.KEYCODE_APOSTROPHE`, `Component.KEYCODE_AT`, `Component.KEYCODE_B`, `Component.KEYCODE_BACK`, `Component.KEYCODE_BACKSLASH`, `Component.KEYCODE_C`, `Component.KEYCODE_CALL`, `Component.KEYCODE_CAMERA`, `Component.KEYCODE_CLEAR`, `Component.KEYCODE_COMMA`, `Component.KEYCODE_D`, `Component.KEYCODE_DEL`, `Component.KEYCODE_E`, `Component.KEYCODE_ENDCALL`, `Component.KEYCODE_ENTER`, `Component.KEYCODE_ENVELOPE`, `Component.KEYCODE_EQUALS`, `Component.KEYCODE_EXPLORER`, `Component.KEYCODE_F`, `Component.KEYCODE_FOCUS`, `Component.KEYCODE_G`, `Component.KEYCODE_GRAVE`, `Component.KEYCODE_H`, `Component.KEYCODE_HEADSETHOOK`, `Component.KEYCODE_HOME`, `Component.KEYCODE_I`, `Component.KEYCODE_J`, `Component.KEYCODE_K`, `Component.KEYCODE_L`, `Component.KEYCODE_LEFT`, `Component.KEYCODE_LEFT_ALT`, `Component.KEYCODE_LEFT_BRACKET`, `Component.KEYCODE_LEFT_SHIFT`, `Component.KEYCODE_M`, `Component.KEYCODE_MEDIA_FAST_FORWARD`, `Component.KEYCODE_MEDIA_NEXT`, `Component.KEYCODE_MEDIA_PLAY_PAUSE`, `Component.KEYCODE_MEDIA_PREVIOUS`, `Component.KEYCODE_MEDIA_REWIND`, `Component.KEYCODE_MEDIA_STOP`, `Component.KEYCODE_MENU`, `Component.KEYCODE_MINUS`, `Component.KEYCODE_MUTE`, `Component.KEYCODE_N`, `Component.KEYCODE_NOTIFICATION`, `Component.KEYCODE_NUM`, `Component.KEYCODE_O`, `Component.KEYCODE_P`, `Component.KEYCODE_PAD_CENTER`, `Component.KEYCODE_PAD_DOWN`, `Component.KEYCODE_PAD_LEFT`, `Component.KEYCODE_PAD_RIGHT`, `Component.KEYCODE_PAD_UP`, `Component.KEYCODE_PERIOD`, `Component.KEYCODE_PLUS`, `Component.KEYCODE_POUND`, `Component.KEYCODE_POWER`, `Component.KEYCODE_Q`, `Component.KEYCODE_R`, `Component.KEYCODE_RIGHT`, `Component.KEYCODE_RIGHT_ALT`, `Component.KEYCODE_RIGHT_BRACKET`, `Component.KEYCODE_RIGHT_SHIFT`, `Component.KEYCODE_S`, `Component.KEYCODE_SEARCH`, `Component.KEYCODE_SEMICOLON`, `Component.KEYCODE_SLASH`, `Component.KEYCODE_SPACE`, `Component.KEYCODE_STAR`, `Component.KEYCODE_SYM`, `Component.KEYCODE_T`, `Component.KEYCODE_TAB`, `Component.KEYCODE_U`, `Component.KEYCODE_V`, `Component.KEYCODE_VOLUME_DOWN`, `Component.KEYCODE_VOLUME_UP`, `Component.KEYCODE_W`, `Component.KEYCODE_X`, `Component.KEYCODE_Y`, or `Component.KEYCODE_Z`)


---

### MenuSelected ###

```
Event MenuSelected(caption As String)
```


> Event raised after a menu entry was selected.

> Parameters:
> > caption - string identifying selected menu item


> Also see [Application.AddMenuItem()](ReferenceLibraryApplication#AddMenuItem.md).


---

### TouchGesture ###

```
Event TouchGesture(direction As Integer)
```

> Event raised after input of a gesture on the touch screen was recognized.

> Parameters:
> > direction - constant identifying direction of touch gesture (one of `Component.TOUCH_DOUBLETAP`,  `Component.TOUCH_FLINGDOWN`, `Component.TOUCH_FLINGLEFT`, `Component.TOUCH_FLINGRIGHT`, `Component.TOUCH_FLINGUP`, `Component.TOUCH_MOVEDOWN`, `Component.TOUCH_MOVELEFT`, `Component.TOUCH_MOVERIGHT`, `Component.TOUCH_MOVEUP` or `Component.TOUCH_TAP`)


---

### BackgroundColor ###

```
Property BackgroundColor As Integer
```


> Reading from the BackgroundColor property returns the current background color of the form. The color value is encoded as _&Haarrggbb_ where _aa_ represents the alpha value (&H00 - transparent to &HFF - opaque), _rr_ represents the red, _gg_ the green and _bb_ the blue component of the color. Writing to the BackgroundColor property will set the background color of the form.

> There are a number of predefined color constants: `Component.COLOR_NONE`, `Component.COLOR_BLACK`, `Component.COLOR_BLUE`, `Component.COLOR_CYAN`, `Component.COLOR_DKGRAY`, `Component.COLOR_GRAY`, `Component.COLOR_GREEN`, `Component.COLOR_LTGRAY`, `Component.COLOR_MAGENTA`, `Component.COLOR_RED`, `Component.COLOR_WHITE` and `Component.COLOR_YELLOW`.

> The default background color for forms is `Component.COLOR_WHITE`.

---

### Height ###

```
Property Height As Integer
```

> Reading from the Height property returns the current height of the form in pixels. For forms the Height property is a read-only property.

---

### Width ###

```
Property Width As Integer
```

> Reading from the Width property returns the current width of the form in pixels. For forms the Width property is a read-only property.

---

### BackgroundImage ###

```
Property BackgroundImage As String
```

> Writing to this property changes the background image shown on the component. The value assigned to this property should be the name of a file in the project's assets directory. This property is write-only.

---

### Layout ###

```
Property Layout As Variant
```

> Reading from the Layout property returns the current layout object instance. For more information about layouts see LinearLayout, TableLayout and FrameLayout. Writing to the Layout property changes the layout to a different layout. The following predefined constants can be used: `Component.LAYOUT_LINEAR`, `Component.LAYOUT_TABLE` or `Component.LAYOUT_FRAME`.

> Note that once components have been added to the form its layout cannot be changed any longer!

---

### Scrollable ###

```
Property Scrollable As Boolean
```

> Reading from the this property indicates whether the contents of the form are scrollable. Writing to this property will make the contents of the form scrollable in case the components of the form do not fit within the height or width of the form.

---

### Title ###

```
Property Title As String
```

> Reading from the this property returns the title shown at the top of the form. Writing to this property changes the title of the form.