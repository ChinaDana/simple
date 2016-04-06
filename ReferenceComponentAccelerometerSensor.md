<sub>namespace com.google.devtools.simple.runtime.components</sub>
# AccelerometerSensor #

Sensor to measure acceleration in 3 dimensions, and also detect shaking.

#### Events ####
[Initialize](ReferenceComponentAccelerometerSensor#Initialize.md)
> Initialization event.
[AccelerationChanged](ReferenceComponentAccelerometerSensor#AccelerationChanged.md)
> > Acceleration change event.
[Shaking](ReferenceComponentAccelerometerSensor#Shaking.md)
> > Shaking event.

#### Properties ####
[Available](ReferenceComponentAccelerometerSensor#Available.md)

> Available property (read-only property).
[Enabled](ReferenceComponentAccelerometerSensor#Enabled.md)
> Enabled property.
[XAccel](ReferenceComponentAccelerometerSensor#XAccel.md)
> X acceleration property (read-only property).
[YAccel](ReferenceComponentAccelerometerSensor#YAccel.md)
> Y acceleration property (read-only property).
[ZAccel](ReferenceComponentAccelerometerSensor#ZAccel.md)
> Z acceleration property (read-only property).

---

### Initialize ###

```
Event Initialize()
```

> Event raised upon component initialization.

---

### AccelerationChanged ###

```
Event AccelerationChanged(xAccel As Single, yAccel As Single, zAccel As Single)
```

> Event raised when the acceleration in any of the 3 dimensions changes.

> Parameters:
> > xAccel - acceleration minus Gx on the x-axis<br>
<blockquote>yAccel - acceleration minus Gy on the y-axis<br>
zAccel - acceleration minus Gz on the z-axis<br>
<hr />
<h3>Shaking</h3></blockquote></li></ul>

```
Event Shaking()
```


> Event raised when the device is being shaken.

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

### XAccel ###

```
Property XAccel As Single
```

> Reading the value of this property returns the most recent x acceleration value. In order for this property to supply meaningful values, the sensor needs to be available and enabled.

> Writing to this property will accelerate the device at the given rate. Use this only in a controlled environment as sudden acceleration may cause severe injury... No, just kidding - this property is read-only.

---

### YAccel ###

```
Property YAccel As Single
```

> Reading the value of this property returns the most recent y acceleration value. In order for this property to supply meaningful values, the sensor needs to be available and enabled. This property is read-only.

---

### ZAccel ###

```
Property ZAccel As Single
```

> Reading the value of this property returns the most recent z acceleration value. In order for this property to supply meaningful values, the sensor needs to be available and enabled. This property is read-only.