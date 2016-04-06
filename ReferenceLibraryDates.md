<sub>namespace com.google.devtools.simple.runtime</sub>
# Dates #

Various date and time related runtime functions.

[DATE\_YEAR](ReferenceLibraryDates#DATE_YEAR.md)
[DATE\_MONTH](ReferenceLibraryDates#DATE_MONTH.md)
[DATE\_DAY](ReferenceLibraryDates#DATE_DAY.md)
[DATE\_WEEK](ReferenceLibraryDates#DATE_WEEK.md)
[DATE\_HOUR](ReferenceLibraryDates#DATE_HOUR.md)
[DATE\_MINUTE](ReferenceLibraryDates#DATE_MINUTE.md)
[DATE\_SECOND](ReferenceLibraryDates#DATE_SECOND.md)
> Date/time interval kind constants.

[DATE\_JANUARY](ReferenceLibraryDates#DATE_JANUARY.md)
[DATE\_FEBRUARY](ReferenceLibraryDates#DATE_FEBRUARY.md)
[DATE\_MARCH](ReferenceLibraryDates#DATE_MARCH.md)
[DATE\_APRIL](ReferenceLibraryDates#DATE_APRIL.md)
[DATE\_MAY](ReferenceLibraryDates#DATE_MAY.md)
[DATE\_JUNE](ReferenceLibraryDates#DATE_JUNE.md)
[DATE\_JULY](ReferenceLibraryDates#DATE_JULY.md)
[DATE\_AUGUST](ReferenceLibraryDates#DATE_AUGUST.md)
[DATE\_SEPTEMBER](ReferenceLibraryDates#DATE_SEPTEMBER.md)
[DATE\_OCTOBER](ReferenceLibraryDates#DATE_OCTOBER.md)
[DATE\_NOVEMBER](ReferenceLibraryDates#DATE_NOVEMBER.md)
[DATE\_DECEMBER](ReferenceLibraryDates#DATE_DECEMBER.md)
> Month constants.

[DATE\_MONDAY](ReferenceLibraryDates#DATE_MONDAY.md)
[DATE\_TUESDAY](ReferenceLibraryDates#DATE_TUESDAY.md)
[DATE\_WEDNESDAY](ReferenceLibraryDates#DATE_WEDNESDAY.md)
[DATE\_THURSDAY](ReferenceLibraryDates#DATE_THURSDAY.md)
[DATE\_FRIDAY](ReferenceLibraryDates#DATE_FRIDAY.md)
[DATE\_SATURDAY](ReferenceLibraryDates#DATE_SATURDAY.md)
[DATE\_SUNDAY](ReferenceLibraryDates#DATE_SUNDAY.md)
> Weekday constant.

[DateAdd](ReferenceLibraryDates#DateAdd.md)
> Adds a time interval to the given date.
[DateValue](ReferenceLibraryDates#DateValue.md)
> Creates a date from the given string.
[Day](ReferenceLibraryDates#Day.md)
> Returns the day of the month for the given date.
[FormatDate](ReferenceLibraryDates#FormatDate.md)
> Converts and formats the given date into a string.
[Hour](ReferenceLibraryDates#Hour.md)
> Returns the hours for the given date.
[Minute](ReferenceLibraryDates#Minute.md)
> Returns the minutes for the given date.
[Month](ReferenceLibraryDates#Month.md)
> Returns the month of the given date.
[MonthName](ReferenceLibraryDates#MonthName.md)
> Returns the name of the month for the given date.
[Now](ReferenceLibraryDates#Now.md)
> Returns the current date and time.
[Second](ReferenceLibraryDates#Second.md)
> Returns the seconds for the given date.
[Timer](ReferenceLibraryDates#Timer.md)
> Returns the current system time in milliseconds.
[Weekday](ReferenceLibraryDates#Weekday.md)
> Returns the weekday for the given date.
[WeekdayName](ReferenceLibraryDates#WeekdayName.md)
> Returns the name of the weekday for the given date.
[Year](ReferenceLibraryDates#Year.md)
> Returns the year of the given date.



---

### DATE\_YEAR ###
### DATE\_MONTH ###
### DATE\_DAY ###
### DATE\_WEEK ###
### DATE\_HOUR ###
### DATE\_MINUTE ###
### DATE\_SECOND ###
```
Const DATE_YEAR As Integer
Const DATE_MONTH As Integer           
Const DATE_DAY As Integer           
Const DATE_WEEK As Integer           
Const DATE_HOUR As Integer           
Const DATE_MINUTE As Integer           
Const DATE_SECOND As Integer           
```
Date/time interval kind constants.

---

### DATE\_JANUARY ###
### DATE\_FEBRUARY ###
### DATE\_MARCH ###
### DATE\_APRIL ###
### DATE\_MAY ###
### DATE\_JUNE ###
### DATE\_JULY ###
### DATE\_AUGUST ###
### DATE\_SEPTEMBER ###
### DATE\_OCTOBER ###
### DATE\_NOVEMBER ###
### DATE\_DECEMBER ###
```
Const DATE_JANUARY As Integer           
Const DATE_FEBRUARY As Integer
Const DATE_MARCH As Integer
Const DATE_APRIL As Integer
Const DATE_MAY As Integer
Const DATE_JUNE As Integer
Const DATE_JULY As Integer
Const DATE_AUGUST As Integer
Const DATE_SEPTEMBER As Integer
Const DATE_OCTOBER As Integer
Const DATE_NOVEMBER As Integer
Const DATE_DECEMBER As Integer
```
Month constants.

---

### DATE\_MONDAY ###
### DATE\_TUESDAY ###
### DATE\_WEDNESDAY ###
### DATE\_THURSDAY ###
### DATE\_FRIDAY ###
### DATE\_SATURDAY ###
### DATE\_SUNDAY ###
```
Const DATE_MONDAY As Integer
Const DATE_TUESDAY As Integer
Const DATE_WEDNESDAY As Integer
Const DATE_THURSDAY As Integer
Const DATE_FRIDAY As Integer
Const DATE_SATURDAY As Integer           
Const DATE_SUNDAY As Integer
```
Weekday constant.


---

### DateAdd ###

```
Static Sub DateAdd(date As Date, intervalKind As Integer, interval As Integer)
```

> Adds a time interval to the given date.

> Parameters:
> > date - date to add to
> > intervalKind - kind of interval (one of DATE\_YEAR, DATE\_MONTH, DATE\_DAY, DATE\_WEEK, DATE\_HOUR, DATE\_MINUTE or DATE\_SECOND)
> > interval - units to add

---

### DateValue ###

```
Static Function DateValue(value As String) As Date
```


> Creates a date from the given string.

> Dates must be formatted as follows:
> MM/DD/YYYY hh:mm:ss
> or
> MM/DD/YYYY
> where MM is the month (01-12), DD the day (01-31), YYYY the year (0000-9999), hh the hours (00-23), mm the minutes (00-59) and ss the seconds (00-59).

> Parameters:
> > value - string to convert

> Returns:
> > date

---

### Day ###

```
Static Function Day(date As Date) As Integer
```


> Returns the day of the month for the given date.

> Parameters:
> > date - date to get day of

> Returns:
> > day (range 1 - 31)

---

### FormatDate ###

```
Static Function FormatDate(date As Date) As String
```


> Converts and formats the given date into a string.

> Parameters:
> > date - date to format

> Returns:
> > formatted date


---

### Hour ###

```
Static Function Hour(date As Date) As Integer
```


> Returns the hours for the given date.

> Parameters:
> > date - date to use hours of

> Returns:
> > hours (range 0 - 23)

---

### Minute ###

```
Static Function Minute(date As Date) As Integer
```


> Returns the minutes for the given date.

> Parameters:
> > date - date to use minutes of

> Returns:
> > minutes (range 0 - 59)

---

### Month ###

```
Static Function Month(date As Date) As Integer
```


> Returns the month of the given date.

> Parameters:
> > date - date to use month of

> Returns:
> > month: DATE\_JANUARY, DATE\_FEBRUARY, DATE\_MARCH, DATE\_APRIL, DATE\_MAY, DATE\_JUNE, DATE\_JULY, DATE\_AUGUST, DATE\_SEPTEMBER, DATE\_OCTOBER, DATE\_NOVEMBER, DATE\_DECEMBER

---

### MonthName ###

```
Static Function MonthName(date As Date) As String
```


> Returns the name of the month for the given date.

> Parameters:
> > date - date to use month of

> Returns:
> > name of month

---

### Now ###

```
Static Function Now() As Date
```


> Returns the current date and time.

> Returns:
> > current date and time

---

### Second ###

```
Static Function Second(date As Date) As Integer
```


> Returns the seconds for the given date.

> Parameters:
> > date - date to use seconds of

> Returns:
> > seconds (range 0 - 59)

---

### Timer ###

```
Static Timer() As Long
```


> Returns the current system time in milliseconds.

> Returns:
> > current system time in milliseconds

---

### Weekday ###

```
Static Function Weekday(date As Date) As Integer
```


> Returns the weekday for the given date.

> Parameters:
> > date - date to use weekday of

> Returns:
> > weekday: DATE\_SUNDAY, DATE\_MONDAY, DATE\_TUESDAY, DATE\_WEDNESDAY, DATE\_THURSDAY, DATE\_FRIDAY, DATE\_SATURDAY

---

### WeekdayName ###

```
Static Function WeekdayName(date As Date) As String
```


> Returns the name of the weekday for the given date.

> Parameters:
> > date - date to use weekday of

> Returns:
> > name of weekday

---

### Year ###

```
Static Function Year(date As Date) As Integer
```


> Returns the year of the given date.

> Parameters:
> > date - date to use year of

> Returns:
> > year