**Tutorial 03**: Version 0.1 (written by Uriel Deveaud - 01/2019) 

[**Return to Main Menu**](../README.md)

![](images/header.jpg)

# Using module´s Template files

As we have a basic understanding of how we will make a new module plugin from a bunch of files, placed in the Correct folder ! 
[**HERE**](files/tutorial_VCV_modules.zip) is the link to download the template files ! Get the archive and uncompress it in your plugins folder... you should be able to access this directory:
```
C:/msys64/home/Rack/plugins/tutorial/
```

Now, lets have a look in detail inside those files. At least, you need only 5 files to make a module:
* _**Makefile**_ = Got all relation data para building the final plugin
* _**MyModule.cpp**_ = Got all the source code of your module
* _**MyProject.cpp**_ = Got all initialization data, shared between modules (if you create more than one)
* _**MyProject.hpp**_ = Got all Project references, common data and shared UI elements
* _**background.svg**_ = The design of your module´s background

## Makefile
```
RACK_DIR ?= ../..

SLUG = Tutorial
VERSION = 0.6.1

FLAGS +=
CFLAGS +=
CXXFLAGS +=
LDFLAGS +=
SOURCES += $(wildcard src/*.cpp)
DISTRIBUTABLES += $(wildcard LICENSE*) res

include $(RACK_DIR)/plugin.mk
```
---

## MyProject.hpp
```c++
#include "rack.hpp"

using namespace rack;

extern Plugin *plugin;

extern Model *modelTUTO_MODULE;
```
---

## MyProject.cpp
```c++
#include "MyProject.hpp"

Plugin *plugin;

void init(Plugin *p) {
	plugin = p;
	p->slug = TOSTRING(SLUG);
	p->version = TOSTRING(VERSION);

	// Add all Models defined throughout the plugin
	p->addModel(modelTUTO_MODULE);

	// Any other plugin initialization may go here.
	// As an alternative, consider lazy-loading assets and lookup tables when your module is created to reduce startup times of Rack.
}
```
---

## MyModule.cpp
```c++
#include "MyProject.hpp"

// ------------------------------------------------------------- VARIABLES
struct tutoModule : Module {
	enum ParamIds {
		//SOME_PARAM,
		NUM_PARAMS
	};
	enum InputIds {
		//SOME_INPUT,
		NUM_INPUTS
	};
	enum OutputIds {
		//SOME_OUTPUT,
		NUM_OUTPUTS
	};
	enum LightIds {
		//SOME_LIGHT,
		NUM_LIGHTS
	};

	tutoModule() : Module(NUM_PARAMS, NUM_INPUTS, NUM_OUTPUTS, NUM_LIGHTS) {}
	void step() override;
};

// ------------------------------------------------------------- FEATURES
void tutoModule::step() {
	// Implement features here !
	
}

// ------------------------------------------------------------- UI
struct tutoModuleWidget : ModuleWidget {
	tutoModuleWidget(tutoModule *module) : ModuleWidget(module) {
		setPanel(SVG::load(assetPlugin(plugin, "res/TutoModule.svg")));

		addChild(Widget::create<ScrewSilver>(Vec(RACK_GRID_WIDTH, 0)));
		addChild(Widget::create<ScrewSilver>(Vec(box.size.x - 2 * RACK_GRID_WIDTH, 0)));
		addChild(Widget::create<ScrewSilver>(Vec(RACK_GRID_WIDTH, RACK_GRID_HEIGHT - RACK_GRID_WIDTH)));
		addChild(Widget::create<ScrewSilver>(Vec(box.size.x - 2 * RACK_GRID_WIDTH, RACK_GRID_HEIGHT - RACK_GRID_WIDTH)));

	}
};

// ------------------------------------------------------------- MODEL
Model *modelTUTO_MODULE = Model::create<tutoModule, tutoModuleWidget>("Tutorial", "tutoModule", "tutorial Module", OSCILLATOR_TAG);

```
