---
id: build_calibration
title: Calibration
sidebar_label: Calibration
---

The official way is explained in the service manual here, if you are using a real CPU you should look at page 8 and first do the CPU timing adjustment, the rest of the adjustments are on the following pages of the service notes or just read on below. <a href="http://privat.bahnhof.se/wb447909/dinsync/service_manuals/TB-303.pdf" target="_blank">http://privat.bahnhof.se/wb447909/dinsync/service_manuals/TB-303.pdf</a>

The “fast” way if you don’t need to calibrate the CPU timer.

First check and set the power level as you did in the build but now with a populated machine you should check that you have the correct 5.333v reference (see the power supply section of this guide)

Next set the tune knob to its middle position. Program a C note and then high octave C note into the sequencer and and set the time mode to play long alternating notes. Connect up your scope to the middle post of the waveform switch and adjust TM5 so that the frequency of the higher C is double that of the lower C.

Now program an A into the sequencer and adjust TM4 so that the frequency is 110hz. You can then check by programming a shifted down A that the frequency is around 55hz and that a shifted up A is reading around 220hz.

Now you need to set the center frequency of the VCF, many people like to set this by ear or open it fully. Personally I think the service notes version is the best way to set this as some filter interaction is lost if this is open fully. So,

Connect scope to TP6  
Set waveform to sawtooth  
Set CUTOFF FREQ to center  
Set RES fully clockwise  
Set ENV MODE, DECAY, ACC fully counter clockwise  
Program A (110hz) as before and observe the waveform as notes are hit, adjust TM3 until you have 2ms gaps between the resonant peaks (see picture on page 7 of the service notes).


Now all that remains is the vca trimming if you fitted the optional trimmer. This is quite simple, once the machine has warmed up, run the sequencer so that notes are playing. Now move the waveform switch half way until the waveform is silent but you hear the chirp and dc thump of the filter and vca. Now adjust the trimmer to minimise the thump (it will always be a small amount).
 
That’s it, by now you should have a working RE-303, information on the dice roll is below. Congratulations on completing the mission Space Cadet!