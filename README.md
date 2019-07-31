ZX81+35
====

ZX81+35 is my clone of the Sinclair ZX81, started in 2014, and finished in 2016, it uses modern (SMT) components on a small (10x10cm) PCB, and only uses commercially available parts, so no ULA, and works with the original ZX81 ROM code.

Previously (in 2014) I named it ZX14 but after two years working on it, I changed my mind and renamed it to first to ZX81+34 and later to ZX81+35 to clarify that my copy was first designed 34/35 years after the original

There are three versions of my clone, the first prototype I designed was called ZX81+34 (Rev 1.0) and was build and tested. This PCB needed many patches, for example the 5V and GND signals on the micro-USB port were inverted, and the footprint for the crystal oscillator I chose was wrong.

The second PCB I made and tested was called ZX81+35 (rev 2.2) and was tested in 2016, and only needed a minor patch to work, and some patches to improve cassette loading. 

The third version (revisions 3 and later) were never tested, but all improvements found were implemented in the layout, and patches tested on the Rev 2.2 PCB. this latest version was rev 4.0
This version fully worked as a ZX81 clone, but was not released because I could not get the turbo (overclocking) to work with a stable picture, so I stalled its release, and eventually I gave up on getting turbo mode to work. And started to work on a color home computer called RhoCoCo, information on that one can be found here:
https://revspace.nl/Designing_the_RhoCoCo_Retro_Home_COlor_COmputer_hardware

This version of ZX81+35 has an expansion port that is corrected and should work with ZX81 peripherals, (using an adapter consisting of a strip of PCB fingers soldered to a female pinheader connector)

It also has an onboard extra 8-bit output port, that can be used to drive an LCD display, and adds 4-bit sound (although these latter options were never tested, but they should individually work with a suitable software driver). The 8-bit output can also be used for general purpose outputs, and there is also one general purpose input

It also has both acceleration features, which enabling can be combined using a dual pole switch located on the back of the board, or can be individually enabled using two jumpers. When loading original cassettes turbo mode should be disabled.

The keyboard supports a reset input, (pressing two buttons simultaniously) as well as turbo and power on LED's, but should otherwise be fully compatible with a real ZX81.

A complete step by step description of the design process with all improvements I did for Rev 4.0 up-to september 2016 can be read here:
https://revspace.nl/ZX81PLUS34_ZX81_clone

release
===
Recently (june 2019) I became aware there is interest in my project, so I'm willing to release the latest schematics, BOM, gerbers and drill files here, so anyone can pick this up and create his own version. For now I uploaded the files I have, some are on an old laptop, so will take some more work.

I updated the older BOM so its compatible with revision 4.0

I also designed a keyboard overlay for a keyboard with 40 6x6mm buttons mounted in a 1/10" raster.
I designed a (single sided) keyboard PCB for it, but never tested it, as my protoype keyboard was simply build up on veroboard, Iḿ reasonably sure though that the keyboard PCB is compatible with rev 4.0, if I can find the old layout and check it for compatibility with Rev 4.0


