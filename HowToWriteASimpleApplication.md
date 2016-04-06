# How To Write A Simple Application #

## Prerequisites ##

The first step is to either download the appropriate Simple distribution for your computer or to download the Simple source code and [build the system yourself](HowToBuildTheSimpleCompiler.md). Either way you will end up with a distribution for writing Simple programs.

In addition to the Simple distribution you also need to have to following software installed on your computer:

  * Java SDK version 1.6 or newer
  * [Android SDK version 1.5 or newer](http://developer.android.com/sdk/1.5_r3/index.html)

This distribution of Simple contains commandline tools only. Currently there are no IDEs that support Simple available. That means that you will have to invoke the Simple compiler from a command shell. In order for the Simple compiler to find all necessary files, you will have to define the following environment variables:

  * JAVA\_HOME needs to point to the root directory of the Java SDK or JRE installation
  * ANDROID\_HOME needs to point to the root directory of the Android installation
  * SIMPLE\_HOME needs to point to the root directory of the Simple distribution

## Simple Language Specification ##

The [Simple Language Specification](http://simple.googlecode.com/files/Simple_Language_Definition.pdf) is neither a tutorial for general programming nor programming in Simple. Nevertheless it contains examples to illustrate the usage of the Simple programming language.

## API Reference ##

See the [Runtime Library Reference](RuntimeLibraryReference.md).

## Component Reference ##

See the [Component Reference](ComponentReference.md).

## Creating A New Project ##

The Simple distribution comes with a tool to create a new Simple skeleton project. Assuming that you also added root directory of the Simple distribution to your PATH environment variable, you can run the following command:

```
newsimpleproject com.mydomain.test.Test
```

This will create a folder name Test in your current directory which contains a new Simple project. The main form for this project can be found in `Test/src/com/mydomain/test/Test.simple`.

## Building And Deploying A Project ##

In order to build a Simple project you need to invoke the Simple compiler with the following command:

```
simplec Test/simpleproject/project.properties
```

This command will compile the project contained within the Test folder. The generated Android application can be found in `Test/build/deploy/Test.apk`. If you want to deploy the application you need to invoke the `adb` tool that is part of the Android SDK:

```
adb install -r Test/build/deploy/Test.apk
```

Should you need to uninstall a previously installed apk file, you can run `adb` with the following commandline (note that in this case you pass the namespace of your application as an argument):

```
adb uninstall com.mydomain.test
```

## Signing an Application for Release ##

By default the Simple compiler signs application with a debug key. This is not sufficient for actually releasing applications. To sign an application for release you need to add two line to the project file which can be found at `Test/simpleproject/project.properties`:

```
key.location=<location of your key file>
key.alias=<key alias>
```

After making these changes you can rebuild your project. You will be prompted for your key password during the build. After the build finished you can deploy your application.

For more information on signing Android applications and key files see the [Android documentation](http://developer.android.com/guide/publishing/app-signing.html).

## Static Forms vs. Dynamic Forms ##

Simple forms can be constructed in two ways: either statically, as part of the source file, or dynamically inside the Initialize event handler of the form.

The [Simple Language Specification](http://simple.googlecode.com/files/Simple_Language_Definition.pdf) describes in its appendix the structure of statically defined forms. Note that layout properties must must be the first properties for a container to be defined ahead of any other properties or any child components.

Dynamic forms must be created in the Initialize event handler of a form. There is a special form of the New operator that instantiates a component as well as places it into its container:

```
Event Test.Initialize()
  Dim table As Panel
  table = New Panel On Test
  table.Layout = Component.LAYOUT_TABLE
  table.Layout.Columns = cols
  table.Layout.Rows = rows
End Event
```

For a larger sample see the [Tetris sample application](HowToWriteASimpleApplication#Tetris.md).

## Sample Applications ##

The Simple source distribution comes with several sample applications which can be found in samples folder:

### EtchSketch ###

A very small program that uses several sensors and a canvas component to simulate an Etch-A-Sketch.

### SpeedDialer ###

Another very small program that just dials a phone number embedded in the source code. Starting the program calls the number. In short: a one-touch dialer.

### Tetris ###

This a little bit larger application of a Tetris-like game. It shows how to create forms dynamically. It also uses gestures to control the falling blocks.