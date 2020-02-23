# Yusynth Ring modulator

http://yusynth.net/Modular/EN/RINGMOD/index.html

All text is from Yusynth

## Description

The balanced modulator or four quadrant multiplier, is a great classical module. it provides the same functions as those of a ring modulator. Its main purpose is to generate  sounds with a complex overtone content such as bell sounds and other klang tones !
The principle of this circuit is based on a Gilbert cell (see references at the end of this page) contained in the classical LM1496 IC.


Basically, if one feeds the A input with a sinewave with frequency f1, that is sin(2πf1), and the B input with a sinewave with frequenc f2, that is sin(2πf2), one gets at the output the product these two signals, that is sin(2πf1) x sin(2πf2).

Due to trigonomic properties it reads :

 sin(2πf1) x sin(2πf2) = sin(2π(f1+f2)) + sin(2π(f1-f2))

in other words the output is a mixture of two sinewaves, one with frequency f1+f2 and the other with frequency f1-f2.

## Schematic

The schematic of this balanced modulator is directly inspired by that of the Elektor's Formant  (which is a mere adaptation of the application schematic of the LM1496 datasheet, see at the end of this page). I have only changed the values of the input resistors in order to make the input signal levels compatible with the Moog/Dotcom standards (10V peak to peak) I also added an output stage that amplifies the output signal by 6.8 in order to obtain 10Vpp.

## Settings and trimming


There are four trimmers to adjust : A1 to A4. These trimmers are used for cancelling the input signals. The settings are quite simple, you will need a signal generator that delivers a sinewave signal with a 10V (peak to peak) output amplitude. Here is how to proceed :
Tune the generator on 1000Hz and set the output level of the generator to 10Vpp.

Connect the output AxB (or CxD) of the module to an audio amplifier. Be sure to set the input potentiometer of the amplifier to a low value : the output level of the module is 10Vpp and most of the audio amplifiers expect an input level that doesn't exceed 1Vpp.
Connect the signal generator to the input A (or C) with a capacitor (AC-INPUT). There, you must hxear the 1000Hz signal at the output AxB (or CxD).

Adjust the trimmer A2 (or A4) such that the 1000Hz signal can no longer be heard at the output.

Disconnect the signal generator from input A (or C) and then connect the signal generator to the input B (or D)  with a capacitor (AC-INPUT). There, you must hear the 1000Hz signal at the output AxB (or CxD).
Adjust the trimmer A1 (or A3) such that the 1000Hz signal can no longer be heard at the output.

Now the module is ready to operate. A last check can be done by connecting the 1000Hz signal to both inputs A and B (AC inputs) : there you must hear a single signal of frequency twice as high (2000Hz).

**Comment (JT): A1 and A3 are the 470/500 ohm pots, A2 and A4 are 200/220 ohm.**