**Tutorial 01**: Version 0.1 (written by Uriel Deveaud - 01/2019) 

[**Return to Main Menu**](../README.md)

# Setup your development environment under Win10

So, let´s start from the beginning, you computer is up to become your building machine, but you need to prepare your setup to be able to build applications. First of all, you will need to download a couple of softwares to perform each tasks, as always, i recommend to get some free or open source applications, but other professional softwares will be fine. Just mind the corresponding download, regarding your operating system, and don´t forget that VCV Rack is only working on 64bits OS !

- **Coding**,  [**Visual Studio Code**](https://code.visualstudio.com/)
- **Drawing**, [**Inskape**](https://inkscape.org/), but it can be done with Adobe illustrator, Gravit, etc... or any on-line SVG Editor
- **Building**, [**MSYS64 and its installer**](https://www.msys2.org/)

Once you have installed those softwares, you need to understand what kind of file´s extension you want to create and execute:

- **.cpp**,  all our code will be written in C++, before it get compiled
- **.svg**, our visuals will be exported as SVG or "vector based graphics"
- **.dll**, our final release will include the plugin file and its image´s folder

If everything is fine, you should be able to open the 3 softwares at the same time. I know that there is an issue if you have some anti-virus applications running, so i recommend to disable it during your installation process !

![](images/1_software.jpg)

Don´t forget to do any necessary updates, you always need the last version ! I suggest you to read carefully this page, regarding Msys64 updates: [**How to update MSYS64 ?**](https://www.msys2.org/)

---

## Downloading the VCV Rack Repository and building the main application

Now, we have to get the source code of VCV Rack, to be able to compile it and to run it of course !
Again, read carefully the VCV documentation page [**VCV documentation page**](https://vcvrack.com/manual/Building.html#setting-up-your-development-environment), and make sure you are completing each steps of the process, it is kind of easy, just follow the guide.
Be aware that from now, most of the commands will be executed thru the Msys64 console terminal, keep it open !

Also, you should have this main VCV Rack directory´s accessible at:
```
C:/msys64/home/Rack/
```
If it not exists, you must create manually the plugins folder:
```
C:/msys64/home/Rack/plugins/
```



## Configuring files and folders

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
