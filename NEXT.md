# Next

MAKE SURE ADDING THE CLASS IN ADD/DROP REQUIRES PERMISSION





## flow

maybe there's just a midterm and a final

I'm wondering if bumping up the exercises a bit, include electronics along the way, and then having the Sound Object as the final. bump up the soundscape assignment a bit too, with added mics (so maybe push it back a bit). and eliminate laser cutting.

artist choices and readings are banging


and need desk crits!

crit for all exercises

yes, just midterm and final

workshop on switches
do a friday session on laser cutting


## Readings

Make them official!

Fred Moten?

## Presentations

download material from student presentations; make sure I'm good on all the artists

go through Moodle to add the "slides such as Keynote" phrase


chavez was great, but what about Victoria Chen??

Christian Marclay? 

chacon and french guy -- whoops I have two birds! take out chacon, this piece is not good.

Leon Theremin?



## Intro

can the intro be a way of teaching transduction, rather than listening? use bodies to make a recording system?

/

or, there chould be something more interesting about the size and nature of sound waves. could that be the hand-on workshop?



## Recording

without numbers, the graphics arent in order so it's a problem to show them -- number everything!

but regardless, this kind of sucked. it needs to be at the least a physical demonstration with a turntable. 

electromagnetism is so central, also, we need to see an electromagnet.

What is Audio! electrical signal that fluctuates in a way that is analogous to a sound wave — and which is then transferred into one (whether or not it originated as one)

digital? == measurements


==> should actually spend time to respond (not necessarily critique) the exercises (what are we hearing?)


### contact mics


add the preamp circuit for them?
https://www.richardmudhar.com/blog/2022/07/piezo-contact-microphone-preamp-for-plug-in-power/

show the images on the display as I go around

CAN WE DO SOMETHING WITH ELECTRETS?

http://www.openmusiclabs.com/learning/sensors/electret-microphones/



## Editing / Arranging

have a demo file for this! I did it without hearing anything, which was ridiculous

note the headphone quirk where it doesnt recognize the device

a chance to have mixing feedback is a bit important

importing multiple source files?

normalize on export

images for Envelopes and Pannin


## Soundscape

move Ernst up to present same day as Cardiff, need a bit more for that class, and can add something else less crucial for understanding soundscapes (add diversity, as that isn't as necessary to understand in advance, pairs with the Robinson)


## Soldering

solder removal with those braided strips


## Amps + Speakers

DFPLayer? ---> for the first "resonating body" exercise, just have them use their recorders. _then_ we introduce DFPlayer for the assignment [hmm, maybe not time for that]

need an image of the wires wrapped in the stereo plug prior to soldering

no one made a box for "resonating body". I think I should demonstrate this with a cardboard box.

also, how transducers are used needs to be demonstrated

and maybe for that exercise we all use the same sound? eh.


### strategies that came up that I noted:
dampening
intimacy
directionality
frequency choice -- treble vs bass
personification
found objects 
movement
vibration of other moving
cymatocs 
different pitch resonates
signifying 
enclosures?
surface moving


## Laser Cutting

Add to tutorial:
- Inkscape segment deletion (make the nodes and then do control-double click)
- Images to the glowforge instructions

I actually wonder if laser cutting takes up too much time that could be used for electronics. not enough people are taking advantage of it anyway.


## Sound Objects

I am anticipated it really needs two full weeks, presenting on the following Monday
which implies that using a final exam period would really help open up the final project possibilities

didnt get a chance for proper desk crits (the other project either)




## circuits

### more on circuits

https://eater.net/8bit

solenoids could really be key. but how does that integrate? and battery power?

### now

oscillators —> synthesizers

the flow diagrams are a little weird if the rail-breadboard is going to be used for mixing.


don't have the pot hanging over the edge in the diagram, they will copy that directly and make more fragile boards

LFO with the other chip



### 

SWITCHES
- turning things on and off with buttons, switches, and custom tin foil contacts would be very helpful
- if this could control the audio player to do different sounds, that would be even better (gets a little bit of interaction without a microcontroller)

[microcontroller class is definitely the next step, course-wise]

MICS
being able to integrate the mics and the speaker circuits would be great

what does that imply? 
- making a spring reverb, say
- or a distortion circuit
- tape delay (if we integrate tapes) ---> take out the field recording portion?

but at the least, feedback and amplifying small mechanical sounds

this requires some kind of preamp situation. would need to work with an electret and the contact at least.


also, a mixer. with a mixer, it could work with the synth electronics.


SWITCHES


heat guns bend plexiglass!


motors / servos



### preamp module

TS jack (different!)
10 uF capacitor
4049

an electret works with the breakout. ideally it would be interchangeable with a version with a jack that worked on the recorder, however. but it doesn't seem to work with the preamp straightup. 


==> piezo works with preamp
==> electret works with plug-in power; not without
==> coil does not work with preamp      [probably impedence?] ---> this is annoying
==> electret does not work with preamp  [also? or?]
==> electret with breakout _does_ work with preamp


https://www.epanorama.net/circuits/microphone_powering.html

https://www.youtube.com/watch?v=F21lvgMFglw


I _could_ use a 9v amp. but that increases the speaker output to 20W, which gets a little too serious.



### sensors

integrate proximity sensor?

//

GO MONO in general


build the 9v into the mic and bypass plug-in power

this is only elegant if I can get the inductor to work with the preamp 

so ... better preamp