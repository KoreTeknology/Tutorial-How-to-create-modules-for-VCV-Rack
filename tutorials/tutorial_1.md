Tutorial 01: Version 0.1

# Setup your development environment under Win10

---

So, let´s start from the beginning, you computer is up to become your building machine, but you need to prepare your setup to be able to build applications. First of all, you will need to download a couple of softwares to perform each tasks, as always, i recommend to get some free or open source applications, but other professional softwares will be fine. Just mind the corresponding download, regarding your operating system, and don´t forget that VCV Rack is only working on 64bits OS !

- **Coding**,  [**Visual Studio Code**](https://code.visualstudio.com/)
- **Drawing**, [**Vectr**](https://vectr.com/), but it can be done with Adobe illustrator, Inskape, Gravit, etc... or any on-line SVG Editor
- **Building**, under Win10 64Bits, we will use [**MSYS64 and its installer**](https://www.msys2.org/)

Once you have installed those softwares, you need to understand what kind of file´s extension you want to create and execute:

- **.cpp**,  all our code will be written in C++, before it get compiled
- **.svg**, our visuals will be exported as SVG or "vector based graphics"
- **.dll**, our final release will include the plugin file and its image´s folder

---

If everything is fine, you should be able to open the 3 softwares at the same time.

<img src="https://github.com/KoreTeknology/Quadraphonic-Plugins-for-VCV-Rack/blob/master/Project/Mockups/protoUI1.jpg" width=90%>


## Install a compiler and text editor

---

## Setup VCV and modules files and folders

---

TOEDIT


### Small title

> Comments or notes

---
LISTS

- [x] Step 1: Setup home page and documentation structure
- [ ] Step 2: Uploading first code parts in documentation
- [ ] Step 3: Making available the module files and builds


- **QuadraTrack**, a Single Mono Input track to 4 outputs with controls and options (or 4x4 matrix...)
- **QuadraMaster**, An master output section with 4 audio inputs/outputs with effects, limiter and options
- **QuadraEngine**, a 4 tracks sequencer, recorder/player, audio/midi from files, with 4 audio channel and 16 Midi channel

---
TABLES

| Date | Title |
| --- | --- |
| **2019-02-19** | Module *QuadraTrack 0.2b* - for **Rack v0.6.2** |

---

IMAGE

<img src="https://github.com/KoreTeknology/Quadraphonic-Plugins-for-VCV-Rack/blob/master/Project/Mockups/protoUI1.jpg" width=90%>

---
LINKS

[Kore Teknology](https://github.com/KoreTeknology)

--- 
CODE

```c++
if (isAwesome){
  return true
}
```
