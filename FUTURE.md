# Introduction to Sound Art

## what's left out
music. composition. internal structure. and/or sonification and data manipulation. this _is_ really "materiality of sound" as much as possible: recording and digital editing, amplification and speakers, electronic synthesis (pushing the recording off the computer would complete that)

## more/other artists
- Abu Hamdan
- Cildo Meireles (https://www.tate.org.uk/art/artworks/meireles-babel-t14041)

## more/other readings
- feld
- moten


## new workshops

### recording
electromagnetism is so central, we also need to see an electromagnet.


### building a recorder
tin foil cylinder?


### tape players / loops

this really would be great, because we're missing exploration of recording medium

this has a mic input:
https://a.co/d/09oqwT0

this is also ideal:
https://www.bhphotovideo.com/c/product/330021-REG/Hamilton_HA_802_HA_802_1_Watt.html


### infrasound/ultrasound

mems!

what is the response range? could they actually work for infrasound/ultrasound?? that would be a whole unit.
https://www.sparkfun.com/products/18011
https://www.sparkfun.com/products/19389
https://www.adafruit.com/product/2716

...except these don't have that range. bummer.


### contact mics
add the preamp circuit for them?
https://www.richardmudhar.com/blog/2022/07/piezo-contact-microphone-preamp-for-plug-in-power/



### reverb?
that would be a cool thing to make


## solenoids 
could really be key. but how does that integrate? and battery power?


## FM transmitter
pirate radio!



## synthesis modules

### LFO
using that original chip


### sensors
integrate proximity sensor?

### preamp integration

being able to integrate the mics and the speaker circuits would be great

what does that imply? 
- making a spring reverb, say
- or a distortion circuit
- tape delay (if we integrate tapes) ---> take out the field recording portion?

but at the least, feedback and amplifying small mechanical sounds

this requires some kind of preamp situation. would need to work with an electret and the contact at least.

also, a mixer. with a mixer, it could work with the synth electronics.





## other 
improve documentation workshop




# testing

## preamp

TS jack (different!)
10 uF capacitor
4049

an electret works with the breakout. ideally it would be interchangeable with a version with a jack that worked on the recorder, however. but it doesn't seem to work with the preamp straight up. 

player:
==> works without preamp. good to go.

piezo:
==> works with preamp. good to go.

inductor:
==> does not work with preamp 
probably impedence? ---> this is annoying

electret:
==> works with plug-in power to recorder; not without
==> electret does not work with preamp
==> electret with breakout _does_ work with preamp
==> build the 9v into the mic then bypass plug-in power on the recorder?
        **does this work?**


https://www.epanorama.net/circuits/microphone_powering.html

https://www.youtube.com/watch?v=F21lvgMFglw


I _could_ use a 9v amp. but that increases the speaker output to 20W, which gets a little too serious.

...but would that solve _all_ of these problems?


so:
--> test if 9v electret works (stereo or not, then?) into the recorder and the MAX
--> see if a stronger preamp can be made that works with the inductor



