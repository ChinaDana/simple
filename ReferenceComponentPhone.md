<sub>namespace com.google.devtools.simple.runtime.components</sub>
# Phone #

Component providing phone-related functionality. There should be only one phone component per form.

#### Events ####
[Initialize](ReferenceComponentPhone#Initialize.md)
> Initialization event.

#### Properties ####
[Available](ReferenceComponentPhone#Available.md)
> Available property (read-only property).

#### Functions ####
[Call](ReferenceComponentPhone#Call.md)
> Places a call to the given phone number.
[Vibrate](ReferenceComponentPhone#Vibrate.md)
> Vibrates the phone.


---

### Initialize ###

```
Event Initialize()
```

> Event raised upon component initialization.

---

### Available ###

```
Property Available As Boolean
```

> This property indicates whether the sensor is available on the device running the application.
> This property is read-only.


---

### Call ###

```
Sub Call(phoneNumber As String)
```

> Places a call to the given phone number.

> Parameters:
> > phoneNumber - phone number in the form of numbers only (no spaces, no dashes etc.)

---

### Vibrate ###

```
Sub Vibrate(duration As Integer)
```


> Vibrates the phone.

> Parameters:
> > duration - duration in milliseconds