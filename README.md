# UGFX on Teensy 3.2

This is an example project that demos using UGFX to drive an SSD1351 OLED display using a Teensy with PlatformIO

- UGFX 2.9
- Teensy 3.2

This project is based on the UGFX teensy demo, but has been implemented with the PlatformIO build system. I found that configuring UGFX is not very intuitive, but with some persistece I was able to figure out how to accomplish it. 

## Project Notes

The secret sauce of this project lies in the library.json files included in the libraries in the lib folder. These files use a build configuration array, inside of which a srcFilter resides. This srcFilter defines where the source files for the library are defined, so that other libraries referencing this library will be able to find the headers and source files necessary. This is a complex system, and changing these in anyway might result in an incompatible build.



