<sub>namespace com.google.devtools.simple.runtime.components</sub>
# LinearLayout #

Layout for placing components horizontally or vertically. When choosing horizontal orientation, the components will wrap vertically if the width of the container is exceeded.

#### Properties ####
[Orientation](ReferenceComponentLinearLayout#Orientation.md)
> Property controlling the layout orientation.


---

### Orientation ###

```
Property Orientation As Integer
```

> This property sets the orientation of the linear layout. The assigned value must be either `Component.LAYOUT_ORIENTATION_HORIZONTAL` or `Component.LAYOUT_ORIENTATION_VERTICAL`.
> This property is write-only.