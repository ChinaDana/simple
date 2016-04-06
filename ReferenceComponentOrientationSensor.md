<sub>namespace com.google.devtools.simple.runtime.components</sub>
# OrientationSensor #

Sensor that can measure absolute orientation in 3 dimensions.

#### Events ####
[Initialize](ReferenceComponentOrientationSensor#Initialize.md)
> Initialization event.
[OrientationChanged](ReferenceComponentOrientationSensor#OrientationChanged.md)
> Event indicating a change in orientation.

#### Properties ####
[Available](ReferenceComponentOrientationSensor#Available.md)
> Available property (read-only property).
[Enabled](ReferenceComponentOrientationSensor#Enabled.md)
> Enabled property.
[Yaw](ReferenceComponentOrientationSensor#Yaw.md)
> Yaw property (read-only property).
[Pitch](ReferenceComponentOrientationSensor#Pitch.md)
> Pitch property (read-only property).
[Roll](ReferenceComponentOrientationSensor#Roll.md)
> Roll property (read-only property).
[Angle](ReferenceComponentOrientationSensor#Angle.md)
> Property indicating the angle of the current device tilt (read-only property).
[Magnitude](ReferenceComponentOrientationSensor#Magnitude.md)
> Property indicating the magnitude of the current device tilt (read-only property).

---

### Initialize ###

```
Event Initialize()
```

> Event raised upon component initialization.

---

### OrientationChanged ###

```
Event OrientationChanged(yaw As Single, pitch As Single, roll As Single)
```

> Event raised when the orientation in any of the 3 dimensions changes.

> Parameters:
> > yaw - angle between the magnetic north direction and the Y axis, around the Z axis (0 to 359). 0=North, 90=East, 180=South, 270=West


> pitch - rotation around X axis (-180 to 180), with positive values when the z-axis moves toward the y-axis.

> roll - rotation around Y axis (-90 to 90), with positive values when the x-axis moves away from the z-axis.


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

### Pitch ###

```
Property Pitch As Single
```

> Reading the value of this property returns the most recent pitch value of the device. In order for this property to supply meaningful values, the sensor needs to be available and enabled. This property is read-only.

---

### Roll ###

```
Property Roll As Single
```

> Reading the value of this property returns the most recent pitch value of the device. In order for this property to supply meaningful values, the sensor needs to be available and enabled. This property is read-only.

---

### Yaw ###

```
Property Yaw As Single
```

> Reading the value of this property returns the most recent pitch value of the device. In order for this property to supply meaningful values, the sensor needs to be available and enabled. This property is read-only.

---

### Angle ###

```
Property Angle As Single
```

> Reading the value of this property returns the angle in which the device is tilted in degrees. For the magnitude of the tilt, use the [Magnitude](ReferenceComponentOrientationSensor#Magnitude.md) property. In order for this property to supply meaningful values, the sensor needs to be available and enabled. This property is read-only.

---

### Magnitude ###

```
Property Magnitude As Single
```

> Reading the value of this property returns a number between 0 and 1, inclusive, indicating how far the device is tilted. For the angle of the tilt, use the [Angle](ReferenceComponentOrientationSensor#Angle.md) property. In order for this property to supply meaningful values, the sensor needs to be available and enabled. This property is read-only.