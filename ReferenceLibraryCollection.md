<sub>namespace com.google.devtools.simple.runtime.collections</sub>
# Collection #

A collection is an ordered set of items. Unlike arrays where all members must have the same data type, collections do not have that restriction.

[Add](ReferenceLibraryCollection#Add.md)
> Adds a new item to the collection.
[Clear](ReferenceLibraryCollection#Clear.md)
> Removes all items from the collection.
[Contains](ReferenceLibraryCollection#Contains.md)
> Checks whether an item is already part of the collection.
[Count](ReferenceLibraryCollection#Count.md)
> Returns the number of items in the collection.
[Item](ReferenceLibraryCollection#Item.md)
> Returns the item at the specified position.
[Remove](ReferenceLibraryCollection#Remove.md)
> Removes an item from the collection.

---

### Clear ###

```
Sub Clear()
```

> Removes all items from the collection.

---

### Add ###

```
Sub Add(item As Variant)
```

> Adds a new item to the collection.

> Parameters:
> > item - item to be added

---

### Item ###

```
Function Item(index As Integer) As Variant
```


> Returns the item at the specified position.

> Parameters:
> > index - item position

> Returns:
> > item

---

### Count ###

```
Property Count As Integer
```


> Returns the number of items in the collection. This is a read-only property.

---

### Contains ###

```
Function Contains(item As Variant) As Boolean
```

> Checks whether an item is already part of the collection.

> Parameters:
> > item - item to look for

> Returns:
> > True if the item is already in the collection

---

### Remove ###

```
Sub Remove(item As Variant)
```


> Removes an item from the collection.

> Parameters:
> > item - item to remove