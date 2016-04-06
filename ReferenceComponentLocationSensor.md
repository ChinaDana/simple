<sub>namespace com.google.devtools.simple.runtime.components</sub>
# LocationSensor #

Sensor that can determines the current location (longitude, latitude, altitude).

#### Events ####
[Initialize](ReferenceComponentLocationSensor#Initialize.md)
> Initialization event.
[Changed](ReferenceComponentLocationSensor#Changed.md)
> Event indicating a change in location.

#### Properties ####
[Available](ReferenceComponentLocationSensor#Available.md)
> Available property (read-only property).
[Enabled](ReferenceComponentLocationSensor#Enabled.md)
> Enabled property.
[HasAltitude](ReferenceComponentLocationSensor#HasAltitude.md)
> Property indicating whether the sensor supports altitude information (read-only property).
[Latitude](ReferenceComponentLocationSensor#Latitude.md)
> Latitude property (read-only property).
[Longitude](ReferenceComponentLocationSensor#Longitude.md)
> Longitude property (read-only property).
[Altitude](ReferenceComponentLocationSensor#Altitude.md)
> Altitude property (read-only property).
[CurrentAddress](ReferenceComponentLocationSensor#CurrentAddress.md)
> Property containing the current street address (read-only property).

---

### Initialize ###

```
Event Initialize()
```

> Event raised upon component initialization.

---

### Changed ###

```
Event Changed(latitude As Double, longitude As Double, altitude As Double)
```

> Event raised when the location changes.

> Parameters:
> > latitude - latitude


> longitude - longitude

> altitude - altitude in feet.


---

### Available ###

```
Property Available As Boolean
```

> This property indicates whether the sensor is available on the device running the application.
> This property is read-only.


---

### Enabled ###

```
Property Enabled As Boolean
```

> Reading from the Enabled property indicates whether the sensor is generating data. Writing to the Enabled property will turn sensor data generation on or off.
> Data generation is enabled by default.

---

### HasAltitude ###

```
Property HasAltitude As Boolean
```

> Indicates whether the location sensor provides altitude information. This property is read-only.

---

### Longitude ###

```
Property Longitude As Double
```

> Reading the value of this property returns the most recent longitude value of the device. In order for this property to supply meaningful values, the sensor needs to be available and enabled. This property is read-only.

---

### Latitude ###

```
Property Latitude As Double
```

> Reading the value of this property returns the most recent latitude value of the device. In order for this property to supply meaningful values, the sensor needs to be available and enabled. This property is read-only.

---

### Altitude ###

```
Property Altitude As Double
```

> Reading the value of this property returns the most recent altitude value of the device. In order for this property to supply meaningful values, the sensor needs to be available and enabled. This property is read-only.

---

### CurrentAddress ###

```
Property CurrentAddress As String
```

> Provides a street address for the current location. If no street address can be found for the current location, an empty string will be returned. In order for this property to supply meaningful values, the sensor needs to be available and enabled. This property is read-only.