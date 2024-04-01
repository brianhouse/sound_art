# Oscillators

## Synthesis

As we have explored, sound is a phenomena that relates perception, vibration, space, and meaning. So far, working with sound has meant listening and recording acoustic signals. To do that, we've also touched eletrical analog audio by assembling microphones, speakers, and amplifiers, and even manipulated things digitally. But sound has always begun with physical movement. 

However, there is another fundamental way in which sound is understood in relation to technology, and that is to create sound directly with electronics, either analog or digital. This is called synthesis. Rather than approach things using the fanciest digital signal processing software on our laptops, we will explore this using the foundational circuitry used in hardware synthesizer design. 

## Circuit

According to the dictionary, in the general sense the word circuit means "a roughly circular line, route, or movement that starts and finishes at the same place." That applies in the electrical sense, too. A circuit is a loop, or rather, it's typically a whole knot of loops, all of which are flowing from "power" back to "ground" and making something happen along the way. Between power and ground, we use positive (+) and negative (-) to indicate the direction of the flow. 

What is flowing? Electrical current (we could also think about it as electrons, but the physics is a little hairy to conceptualize as those go backwards).

What is flowing? Voltage.

Breadboard review


## Preparation

To make a synth, we will still need an amplifier + speaker like we've used before. The difference is that instead of an audio input jack, we will be wiring in our circuit directly. 

Position an amplifier breakout board at the right end of a large breadboard. We will also need a speaker. For our purposes at the moment, we will just use one, wired to the "L" output. Make the following connections to the power rail: VDD → +, GND → -.

To get going with power, plug in a JST breakout (making sure to align + and - to the markings on the rail), but put it all the way to the left. Use two jumper wires to bridge the two power rails so that we have + and - across the whole breadboard. Then go ahead and plug in a 3xAA battery pack.

[IMAGE]

Circuit-wise, what we have here is one loop that powers the amp.


## Volume Knob

Next we're going create a circuit/loop that is the input signal to the amplifier. The end of that loop is ground, so let's connect L- → -.

Now we need something to flow into L+. But before we do anything else, we're going to add a volume knob. These have three legs—one side is the input, the middle is the output, and the other leg is the ground. What's happening here is that our signal will come to the knob and be divided into two streams—one goes to the amp, and the other goes to ground without reaching it. Turning the knob adjusts the proportion between the two—the higher the voltage that is flowing into the amp, the higher the volume. This is called "voltage dividing".

A "knob" is properly known as a potentiometer (or "pot"), which is also properly known as a **voltage divider**.

[IMAGE]

We haven't made a circuit yet, however, because the input is still hanging. but this is where we attach our signal.


## VCO

The **V**oltage **C**ontrolled **O**scillator is one of the most basic components of a synth. At one time, it was made with vacuum tubes or individual transistors; now, it comes as an IC (**I**ntegrated **C**ircuit) chip. We will be using the CMOS 4046, which looks like this:

[4046]


What it does (lots of things)

[square wave]

Each of the pins has a function

[pin labels]

plug it in carefully, spanning the groove in the middle of the breadboard
will have to bend the legs inward a little bit


### power

power and ground


### freq range

set frequency range: ground + cap	

what is a capacitor?

### freq center

what is a resistor

leaks away to ground ... but not too much

### pitch

variable resistor!

so here is where we have some fun.

#### pot

#### photocell

sensor is between in and out, resistor is between out and ground


#### fsr

### LFO?


## sequencer





use the sequencer for tones and sequencing, how both?

if it's driven by the oscillator, I can get tones -- I need the pot set up for that

if it _drives_ the oscillator, it can gate it.





building a switch:

strip and twist
join the grounds


diagrams:

put in the 68k
put in the filter