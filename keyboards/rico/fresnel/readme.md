# Fresnel TKL PCB

This is an ongoing collaborative effort between me(Rico) and Gondolindrim to provide in a future PCBs using optical technology.  
The core technique used for the PCB has to be credited to Gondolindrim who found the magic trick to have good latencies while not eating a lot of power.  
On the Fresnel TKL PCB I experimented a few hardware things that may in the future be kept in the final design (or not).

As a personal goal I wanted to have an optical PCB for my Frog, hence why I worked on this ;)



* Keyboard Maintainer: [Eric Becourt, aka Rico](https://github.com/mymakercorner)
* Hardware Supported: Fresnel TKL Rev1.1 PCB
* Hardware Availability: not publicly available yet but the plan is to make it open source in the future, so that anyone can easily design optical PCBs.

Make example for this keyboard (after setting up your build environment):

    make rico/fresnel:default

Flashing example for this keyboard:

    make rico/fresnel:default:flash

See the [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) and the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information. Brand new to QMK? Start with our [Complete Newbs Guide](https://docs.qmk.fm/#/newbs).

## Bootloader

You can enter the bootloader in 5 ways:

* **QMK software ways:**
    * **(NOT WORKING YET)Bootmagic reset**: hold down the key at (0,0) in the matrix (the top left key or Escape) and plug in the keyboard
    * **Keycode in layout**: press the key mapped to `QK_BOOT` that is the top left key or Escape on layer 2
    * **Physical RUN button**: double tap the RUN button
* **Native RP2040 MCU ways:**
    * **Physical RUN and BOOT button**: while keyboard is plugged maintain BOOT button pressed, press RUN button then release the BOOT button
    * **Physical BOOT button**: maintain BOOT button pressed while plugging in the keyboard
