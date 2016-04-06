# Contributing to Simple #

## Coding Style ##

Programs are much easier to maintain when all files have a consistent style. We follow the standard Java coding style, as defined by Sun in their  [Code Conventions for the Java Programming Language](http://java.sun.com/docs/codeconv/html/CodeConvTOC.doc.html), with a few exceptions and additions. This style guide is comprehensive and detailed and is in common usage in the Java community.

In addition, we enforce the following style rules:

  1. One top level class per file: There must be exactly one top level java class per .java file.
  1. Imports: Fully qualify imports
  1. Order of imports: google; third party alphabetical ; java(x)
  1. JavaDoc for at least all public methods and fields
  1. Field declarations should be at the top of the file
  1. Indentation: 2 spaces (or 4 if that leads to confusing code), no tabs.
  1. Line length: 100 columns
  1. Comments: Inside of methods use // exclusively
  1. Acronyms are words: Treat acronyms as words in names, yielding XmlHttpRequest, getUrl(), etc.
  1. TODO style: "TODO: Write this description."
  1. Member variable naming: don't use s/m prefixes or underscore suffixes
  1. File encoding: Use UTF-8
  1. Consistency: Look at what's around you!
  1. Warnings: Code must compile warning free
  1. Exceptions: Never catch and ignore them without explanation
  1. Exceptions: do not catch generic Exception
  1. Assertions: Never write code that assumes that assertions are enabled
  1. Finalizers: generally don't use them

## Testing Changes ##

The most important rule of all: **No code submission without running all tests and passing them!** Broken submissions will be rolled back immediately.

There is two kinds of tests. The first kind tests the compiler and the runtime libraries. To run them execute the following command:

```
ant clean runtests
```

The second kind test the components. For this you need to build the test application, deploy it to a device and manually/visually check that all components still behave and look as expected. The commands for the component tests are:

```
${SIMPLE_HOME}/simplec  ../../tests/com/google/devtools/simple/runtime/DeviceTests/StartTests/simpleproject/project.properties
${ANDROID_HOME}/tools/adb install -r ${SIMPLE_HOME}/../../tests/com/google/devtools/simple/runtime/DeviceTests/StartTests/build/deploy/StartTests.apk
```

Whenever fixing bugs or writing new code make sure there is a test accompanying the change.

## Writing Libraries and Components ##
For information on writing new Simple runtime libraries and components see the [Simple Component Writer's Guide](http://simple.googlecode.com/files/Simple_Component_Writer_s_Guide.pdf).