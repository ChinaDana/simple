# How To Build The Simple Compiler and Runtime Library #

## Requirements ##

Before attempting to build the Simple compiler and runtime library, you need to have the following software installed on your computer:

  * Java SDK 1.6 or newer
  * Android SDK 1.5 or newer
  * Ant version 1.7 or newer

## Setup ##

After downloading or checking out the Simple source code, you need to set following environment variables:
  * JAVA\_HOME needs to point to the root directory of your Java SDK installation
  * ANDROID\_HOME needs to point to the root directory of your Android SDK installation
  * SIMPLE\_HOME needs to point to the root directory of the Simple source distribution plus `/dist` plus the one of `/linux`, `/mac` or `/windows` (e.g. `/home/name/simple/dist/linux`)

## Building ##

On Mac or Linux execute the following commands:
```
cd <root of your Simple source distribution>
ant clean all
chmod +x ${SIMPLE_HOME}/simplec
```

On Windows execute the following commands:
```
cd <root of your Simple source distribution>
ant clean all
```

The built Simple compiler can now be found in SIMPLE\_HOME. On Windows its name is `simplec.bat`, on Mac or Linux it is simply `simplec`.