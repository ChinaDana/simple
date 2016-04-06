<sub>namespace com.google.devtools.simple.runtime.components</sub>
# Timer #

Component providing timer functionality.

#### Events ####
[Initialize](ReferenceComponentTimer#Initialize.md)
> Initialization event.
[Timer](ReferenceComponentTimer#Timer.md)
> Timer expiration event.

#### Properties ####
[Enabled](ReferenceComponentTimer#Enabled.md)
> Enabled property.
[Interval](ReferenceComponentTimer#Interval.md)
> Timer interval property.


---

### Initialize ###

```
Event Initialize()
```

> Event raised upon component initialization.

---

### Timer ###

```
Event Timer()
```

> Event raised upon Timer expiration. After completing an event handler for this event, the timer will be reset to the current interval value and restarted (unless it was disabled).

---

### Enabled ###

```
Property Enabled As Boolean
```

> Reading from the Enabled property indicates whether the timer is running and will be restarted after interval expiration. Writing to the Enabled property will turn timer on or off.

> The timer is enabled by default.

---

### Interval ###

```
Property Interval As Integer
```

> Reading from the Interval property returns the number of milliseconds between timer events. Writing to the Interval property will changed the length of the interval between timer events. If the timer is enabled and the interval is being changed then the current timer run is aborted and the timer is immediately restarted with the new interval.

> The default interval is 1000 ms.

---
