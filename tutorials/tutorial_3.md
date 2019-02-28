**Tutorial 03**: Version 0.1 (written by Uriel Deveaud - 01/2019) 

[**Return to Main Menu**](../README.md)

![](images/header.jpg)

# Using module´s Template files

As we have a basic understanding of how we will make a new module plugin from a bunch of files, placed in the Correct folder ! 
[**HERE**](files/tutorial_VCV_modules.zip) is the link to download the template files ! Get the archive and uncompress it in your plugins folder... you should be able to access this directory:
```
C:/msys64/home/Rack/plugins/tutorial/
```

Now, lets have a look in detail inside those files. At least, you need only 4 files to make a module:
* _**Makefile**_ = Got all relation data para building the final plugin
* _**MyModule.cpp**_ = Got all the source code of your module
* _**MyProject.cpp**_ = Got all initialization data, shared between modules (if you create more than one)
* _**MyProject.hpp**_ = Gor all Project references, common data and shared UI elements

## Makefile
```
# If RACK_DIR is not defined when calling the Makefile, default to two directories above
RACK_DIR ?= ../..

# Must follow the format in the Naming section of
# https://vcvrack.com/manual/PluginDevelopmentTutorial.html
SLUG = Tutorial

# Must follow the format in the Versioning section of
# https://vcvrack.com/manual/PluginDevelopmentTutorial.html
VERSION = 0.6.1

# FLAGS will be passed to both the C and C++ compiler
FLAGS +=
CFLAGS +=
CXXFLAGS +=

# Careful about linking to shared libraries, since you can't assume much about the user's environment and library search path.
# Static libraries are fine.
LDFLAGS +=

# Add .cpp and .c files to the build
SOURCES += $(wildcard src/*.cpp)

# Add files to the ZIP package when running `make dist`
# The compiled plugin is automatically added.
DISTRIBUTABLES += $(wildcard LICENSE*) res

# Include the VCV Rack plugin Makefile framework
include $(RACK_DIR)/plugin.mk
```
