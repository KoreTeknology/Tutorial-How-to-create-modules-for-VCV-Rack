# Tutorial: How to create modules for VCV-Rack
Trainings and tips on how to build your own virtual instrument for the VCV Rack platform.

by uriel Deveaud - 2019

---

## Introduction

So, you want to create your own instruments or module in VCV Rack, Welcome on board !

Before we start talking about computer programming, let´s have a look at the general profile and basic knowledge you may need during the process of creating your plugin. right now, you have an idea, and i´am sure, the best one ! As a musician, you may have been diving into some sort of code... or not ! 

Basically, musicians don´t like to loose their time into coding work, but there are exceptions of course.
In this case, you want to join the group of musician-developper, and that´s fine. We will progress step by step and go from a basic module to very complexe ones.

If you are very new to audio programming, c++ and SVG design, you can still follow those tutorials, but i suggest you to be very curious and engaged regarding learning the bases or any introductions that you may see on  youtube or other forums and facebook pages... ask, search and take notes ;) By entering into module creation, there is 99% chance that you will produce more than one plugin, so, take it seriously, learn by method, stay organized, go step-by-step, respect yourself... and you will see, slowly, your instrument coming alive !, the price is nothing compared to the full satisfaction of creating your dream´s device and turning it on for the very first time :)

Well, let´s have a look at this tutorial´s menu. Each section presents various tasks that you want to repeat as necessary, depending of your personal project. So first, you need to know about the "VCV modules API code structure", to know how to compile a plugin and finally to test your creation "live" in VCV Rack. Once this cycle is understood, you are ready to developpe your module´s features and users interface (UI). As just said, we are progressing, following these 3 steps in loop: 

* Looking for code expressions and understanding the "rules"
* Adapting the code rules to the actual needs
* Duplicate and clean code sections

Of course, after some times, you will build your own codes library and you will be able to jump quickly to the next level !
One common suggestion, and it is very important, if you are not an experienced programmer, to "explore" other Module´s codes from their authors pages. From them, you will learn what solution they were choosing and what is the result. You can download their repositories and build them on your local machine. Great teaching, but at least, you need to understand what you are reading :) Let´s reach this objective together with this tutorials serie. Enjoy !

## Summary

1. Prerequisites
   - **Tutorial 01:** Setup your development environment under Win10 [**> Read the tutorial**](tutorials/tutorial_1.md)
     - _Install a compiler and text editor_
     - _Setup VCV and modules files and folders_
     - _Build VCV Rack from scratch_
 
 ---
 
2. Building your First complete module, using Template files
   - **Tutorial 02:** build and test the classic VCV Template > [LINK](https://github.com/KoreTeknology/Quadraphonic-Plugins-for-VCV-Rack/blob/master/Documentation/tuto1.md)
     - _Download the Template files_
     - _Build and test the module in VCV Rack_
   - **Tutorial 03:** Use the new tutorial´s template > [LINK](https://github.com/KoreTeknology/Quadraphonic-Plugins-for-VCV-Rack/blob/master/Documentation/tuto1.md)
     - _Set basic module settings files and folders_
     - _Build and store new modules_
     - _Test your module in VCV Rack_

---

3. Organizing your work and planning tasks
   - **Tutorial 04:** Consolidating and validating your project > [LINK](https://github.com/KoreTeknology/Quadraphonic-Plugins-for-VCV-Rack/blob/master/Documentation/tuto1.md)
     - _Check for similar existing plugins_
     - _Draw some mockups and define features_
   - **Tutorial 05:** Are you ready ? if yes, time to work > [LINK](https://github.com/KoreTeknology/Quadraphonic-Plugins-for-VCV-Rack/blob/master/Documentation/tuto1.md)
     - _Setting up your SLUG, ModuleName, and files_
     - _Defining size and style for your module_

---

4. Building your first created module
   - **Tutorial 06:** Building basic components > [LINK](https://github.com/KoreTeknology/Quadraphonic-Plugins-for-VCV-Rack/blob/master/Documentation/tuto1.md)
     - _Objective, creating a simple audio circuit, aka "THE MIXER"_
     - _Creating Input and outpout ports_
     - _Creating a knob that controls a num param_
     - _Creating a switch button to change a boolean param_
     - _Creating a vu meter to visualize a num param_
     - _Creating a screen to visualize any param_
     - _Creating a momentary button_
     - _Creating a menu with static infos_
     - _Creating a user´s dynamic info on panel_
   - **Tutorial 07:** Customizing your components > [LINK](https://github.com/KoreTeknology/Quadraphonic-Plugins-for-VCV-Rack/blob/master/Documentation/tuto1.md)
     - _Creating your background layer_
     - _Creating new controls_
     - _Creating a screen panel_
     - _Adding some conditional infos in the menu_
     - _Adding some folders for presets_

---

5. Building an advanced module
   - **Tutorial 08:** Creating an audio source > [LINK](https://github.com/KoreTeknology/Quadraphonic-Plugins-for-VCV-Rack/blob/master/Documentation/tuto1.md)
     - _Objective, creating a new audio circuit, aka "THE SAMPLER"_
     - ...
   - **Tutorial 09:** Creating a wave generator > [LINK](https://github.com/KoreTeknology/Quadraphonic-Plugins-for-VCV-Rack/blob/master/Documentation/tuto1.md)
     - _Objective, creating a new audio circuit, aka "THE SYNTHETIZER"_
     - ...
   - **Tutorial 10:** Creating a filter section > [LINK](https://github.com/KoreTeknology/Quadraphonic-Plugins-for-VCV-Rack/blob/master/Documentation/tuto1.md)
     - _Objective, creating a new audio circuit, aka "THE EQUALIZER"_
     - ...
  
---

...

- i am looking for people who can help to extend this documentation on building modules on MacOS and Linux ;)

