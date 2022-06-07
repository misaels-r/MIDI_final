# MIDI_final
Light-controlled midi
Introduction 

MIDI, is an acronym for musical instrument digital interface standardized in 1983. MIDI refers to a digital language shared by computers and some electronic instruments. Computers play back MIDI data using software or devices, called sequencers, which are designed to read MIDI information. The data can be composed on the computer itself or performed on a MIDI musical instrument, called a controller, and then sent to the sequencer.

A MIDI controller is a device used to send MIDI data to a computer or other hardware. In more basic terms, it’s a controller that is used to trigger sounds from an external source. The most common MIDI controllers are undoubtedly keyboards, but we can find guitars, drums, even bagpipes for sale.


Objective: 

Create a midi controller which allows light control. The purpose of this is to include the ambience in which it is used as part of the controller’s parameters and to induce an amount of randomness to its output values. The controller will then be used in a recorded musical performance. 

List of components: 

Software
Ableton Live 
Hairless MIDI Serial Bridge
Arduino IDE

Hardware
Arduino UNO 
Protoboard 
22 Jumper cables 
2 (10k) Resistors
2 Photoresistors 
8 Pushbuttons 


Software download instructions: 

Daw

Firstly we need to install the needed software. In this particular example Ableton Live is used for demonstration purposes but any DAW that allows midi mapping should work as well. 
In case you do not have any DAW, you can try Ableton Live for 90 days, the trial is free and available for both MacOS and Windows.
[https://www.ableton.com/en/trial/?mtm_campaign=16141417401&mtm_kwd=ableton%20live&mtm_source=google&mtm_medium=cpc&mtm_cid=16141417401&mtm_group={AdGroupName}&gclid=Cj0KCQjw4uaUBhC8ARIsANUuDjU2mqeRnaNw3E_u7HABPvhnM5NT7WmtRDkeC774kzl2sfORWWqbsOkaAjb5EALw_wcB Link for download].

Hairless- MIDI

Hairless-MIDI serial bridge is a free software available for both MacOS and Windows which allows the reception of midi messages from serial devices. [http://projectgus.github.io/hairless-midiserial/?source=post_page--------------------------- Link for download].

Arduino IDE

The Arduino IDE is also a free software that will allow us to upload codes to our physical Arduino UNO. 
[https://www.arduino.cc/en/software Link to Arduino’s software website] 
Once installed, compile and upload the arduino code from the repository. 

Connecting to the DAW

Once the software is installed, the program is uploaded to the Arduino and the hardware is assembled as shown in the schematic. We must open both our DAW and Hairless-MIDI. It is important to remember that for the communication to work, both applications must be opened at all times. 

As an extra step if you are working on a Mac, go to Audio MIDI Setup and type in command+2 or go to “window” and select “Show MIDI Studio”. Once there you should see a red rectangle labeled IAC Driver. Double click on the rectangle and add a port. Once done select apply. 

Inside Hairless-MIDI we will select the port in which our Arduino is connected.  
Now, inside Ableton Live (for other DAWs check MIDI mapping options). Click on the MIDI button on the superior right corner. 

Once MIDI mapping mode is activated you can click on anything you want to activate via midi and then interact with your device. 
Ableton will associate the midi message with the action instantly. In the performative example buttons are used to trigger and stop events while photoresistors are mapped to FX parameters (frequency shift and High-frequency cutoff). 

Performance video link: 
https://youtu.be/Kb0slS_CzYc 




