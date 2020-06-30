ZX81+35
====

ZX81+35 is my clone of the Sinclair ZX81, started in 2014, and finished it 2016, (except for turbo mode which I never got to work while producing a perfect picture quality). It uses modern (SMT) components on a small (10x10cm) PCB, and only uses commercially available parts, so no ULA, and works with the original ZX81 ROM code, and has the maximum possible of 32K of RAM buit in. it supports the back-porch patch which makes it better compatible with modern TV's for clear bright and sharp video.

Its called ZX81plus35 here on github because github doesn't allow for the plus sign in project names.

Previously (in 2014) I named it ZX14 but after two years working on it, I changed my mind and renamed it to first to ZX81+34 and later to ZX81+35 to clarify that my copy was first designed 34/35 years after the original.

There are three versions of my clone, the first prototype I designed was called ZX81+34 (Rev 1.0) and was build and tested. This PCB needed many patches, for example the 5V and GND signals on the micro-USB port were inverted, and the footprint for the crystal oscillator I chose was wrong.

The second PCB I made and tested was called ZX81+35 (rev 2.2) and was tested in 2016, and only needed a minor patch to work, and some patches to improve cassette loading. This version fully worked as a ZX81 clone, and was compatible enough to run everything I threw at it, including high resolution graphics.

The third version (revisions 2.3 and later) were never tested, but all improvements found were implemented in the layout, and patches tested on the Rev 2.2 PCB. Rev 2.3 contains the patches I found when testing rev 2.2, the latest version was rev 4.0 which has an 180 degrees rotated expansion header, for full compatibility with the real ZX81, and my PSG board.

It was not released when rev 4.0 was ready, because I could not get the turbo (overclocking) to work with a stable picture, so I stalled its release, and eventually I gave up on getting turbo mode to work, as I started to work on a color home computer of my own design called RhoCoCo, information on that one can be found here:
https://revspace.nl/Designing_the_RhoCoCo_Retro_Home_COlor_COmputer_hardware

So revision 4.0 of ZX81+35 has an expansion port that is corrected and should work with ZX81 peripherals, (using an adapter consisting of a strip of PCB fingers soldered to a female pinheader connector) and directly on my own peripherals (I designed a version of the ZON PSG board for it) https://revspace.nl/Zon_X-81_Programmable_Sound_Generator_expansion_for_ZX81PLUS35. 

The PCB for my ZON compatible PSG with support for an SD-card reader can be find here on github https://github.com/mahjongg2/PSG-for-ZX81-35-ZX81-clone.
Note that it was the last thing I designed for my ZX81 clone, and it was not tested, as it would only work with the corrected expansion port (the revision 4 board).
it should work, and be compatibe with a ZON, and with an adapter, with a real ZX81.

The pin-header edge connector should eliminate the infamous unreliability (wobble) of the expansion connector. Its location on the side of the board (instead of the back) is chosen so that like Sinclairs Quantum leap computer expansion packs can reside within the enclosure of the computer. 

The ZX81+35 also has an onboard extra 8-bit output port, that can be used to drive an LCD display, and adds 4-bit sound (although these latter options were never tested, but they should individually work with a suitable software driver). The 8-bit output can also be used for general purpose outputs, and there is also one general purpose input.

It also has both acceleration features, which enabling can be combined using a dual pole switch located on the back of the board, or can be individually enabled using two jumpers. When loading original cassettes turbo mode should be disabled.

The keyboard supports a reset input, (pressing two buttons simultaniously) as well as turbo and power on LED's, but should otherwise be fully compatible with a real ZX81.

A complete step by step description of the design process with all improvements I did for Rev 4.0 up-to september 2016 can be read here:
https://revspace.nl/ZX81PLUS34_ZX81_clone

release
===
Recently (june 2019) I became aware there is interest in my project, so I'm willing to release the latest schematics, BOM, gerbers and drill files here, so anyone can pick this up and create his own version. For now I uploaded the files I have, some are on an old laptop, so will take some more work.

I updated the older BOM so its compatible with revision 4.0

This design was developed with Ultiboard, (now National instruments NI Ultiboard) the schematic is released as a .UTSCH file, and the layout as .ewprj, hopefully they can be opened with a recent version of NI Ultiboard. I used a version of Ultiboard before they were aquired by NI, but I did not try newer versions. Its one reason why I switched to KiCad.

The revision 4.0 files released here were never turned into a PCB, and tested, but because revision 2.2 was working fine after some patches, and the only difference toward rev 4 was the patches I added to Rev 2.2, and rhe reversal of the expansion connector, I have no doubt version 4.0 will work fine, netlist checking against the schematic, and error checking makes me sure of that.

To ease the assembly I constructed an assembly drawing showing which components go where on the PCB, use it together with the Schematic, and Bill of Materials (BOM) to build up the PCB.

Obviously I would love to have some feedback if you choose to build my ZX81 clone, you can reach me on the Raspberry PI forum, in this thread:
https://www.raspberrypi.org/forums/viewtopic.php?f=62&t=77429

I designed a Keyboard PCB in the form of a 2.5 inch by 6.2 inch single sided PCB, with 40 6x6mm buttons mounted in a 1/10" raste, and uploaded the gerber/drill files here.
I also designed a keyboard overlay for it, you can print it on an A4 sheet, and it should fit the PCB.

best way to use the keyboard overlay is to glue it to thin cardboard, and to laminate this with transparent plastic, then punch out the 40 3.5mm holes for the key plungers to stick through. the keyboard uses fourty industry standard 6x6 mm (6.5 mm wide pitch by 4.5mm high pitch) keys, with 3.5 mm round plungers, a reset button can be attched to it, and it has two 3mm LED's a power LED, and a (currently unused) "turbo" LED.
the keyboard can be connected to the ZX81+35 (or to a real ZX-81) with flat-flex cables (1/10" pitch flat cables).
A real Z80 only uses one 5-wire section, and one 8-wire section, The ZX81+35 uses one 18-wire flat-flex FST-22A cable with some wires removed. Alternatively you can used male and female angled headers for a stiffer interconnect.

If you need help with solving a problem you have with building my ZX81+35 clone, you can reach me at mahjongg commercial-at xs4all.nl. I will be glad to help.

P.S. a previous version of the component overview drawing contained an error, U13 was depicted as a 74HC32, it should in fact be a 74HC00. The drawing has been deleted and a new one uploaded.
I also uploaded a new BOM (bill of materials) in .xlsx format the previously uploaded BOM wasn't downloadable, and if you managed to make sense of the file jumple a download produced also contained an ommission.

The .ZIP with production files now contains a new silk screen file with the text TURBO / NORMAL corrected.`

In july 2020, during the corona crisis, I was contacted by someone who tried to build a ZX81+35, and warned me that there were conflicts between the top-copper layer and the to soldermask. I investigated the matter, and discovered that the .ZIP file contained an older version of the solder mask.

So I repaired the gerber files which now are revision 1.4. If you have downloaded an older version, please throw it away, and use the revision 1.4 Version, or if you already made PCB'(s) use an xacto knife (chirurgical blades) to remove the solder mask of the components that are covered in the top right corner.

My apologies.

## Licence

Unless otherwise specified, everything in this repository is covered by the following licence:

[![Creative Commons Attribution-ShareAlike 4.0 International](http://i.creativecommons.org/l/by-sa/4.0/88x31.png)](http://creativecommons.org/licenses/by-sa/4.0/)

