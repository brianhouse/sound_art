# Editing


There are two mediums in which we can edit audio—magnetic tape, and digital. Many of the artists we've talked about so far have used tape, and to edit tape means literally cutting it and taping the pieces back together. We're going to do things digitally, using Audacity.

Audacity is an open source program and is free to use. In some ways, it is clunkier than commercial production software, but it is also super powerful and can do things that other programs cannot. It is not intended to be a music production tool like Logic or Protools or GarageBand or whatever, but is about directly manipulating recordings and really inherits this model from tape editing.

## Download and install

Download [Audacity](https://www.audacityteam.org)

Drag the application from the DMG folder into the Applications folder on your computer.

Open Audacity, and Choose "File → Import → Audio..." and select your audio file from your computer. If you get a warning dialog box about importing uncompressed audio files, choose the "safer" option and select "Don't warn again":

![](media/03_00_warning_import_uncompressed_audio.png)

Once you've loaded a file, save your Audacity project, "File → Save Project → Save Project". You'll get a warning telling you this saves a project, not a listenable audio file, and that's fine, that's what we want (you can click "Don't show this warning again" if you like). Save it as "edit_exercise.aup" to your computer.

(If you haven't already, I suggest that everyone makes a folder on their computer for this class where you can copy recordings as well as project files. I find that many students these days are so used to using Google Drive that organizing things locally on their computers is new and awkward. Please ask questions if you get lost with things like saving and moving files.)

(Also saving. I have a twitch at this point to hit Command-S, and it's one that you should develop. Save your project file.)

## Lay of the land

Ok, so what do we have here?

It's a waveform representation of the sound. You have two sounds grouped together, because it's stereo. You have time in seconds, and you have amplitude expressed in terms of maximum and minimum.

On the left, it shows the sample rate and bit depth, but you'll notice it's converted the bit-depth to 32-bit float, which is even higher resolution than we recorded it at.

- Cursor  
- Magnifying glass (hold down shift to zoom out)—Zoom all the way in until you see the samples
- ...And at this point, you can actually draw them directly with the draw tool.
- You can use this to directly repair distortion and clicks

## Splicing

So the first thing you want to do is to delete the sections you don't want to work with. This could be because the audio is damaged, or it could be that it's just not a section you're interested in. **This wont affect the original audio file**—that's why we saved this as an audio project.

Use the select tool to select the audio. If the unwanted audio is at the very beginning or the end, you can just hit delete. But if it's in the middle, use: "Edit → Remove Special → Split Delete"

This leaves a blank space. You can then recombine the two sections with a short _crossfade_ by select a bit of audio from each clip on either side of the gap. Then choose "Effect → Crossfade Clips"

Crossfading is critical. We've seen that we need a smooth waveform, otherwise it will produce distortion.

If you have a gap at the beginning of the project, you can use the <-> tool to fix that.

## Processing

Once we have a clean take, with all the pops removed, we're going to do some more post-processing to make things sound better.

#### Prep self-noise

This is also where that self-noise recording comes in. Make sure you've saved this project, and then let's open up your self-noise recording.

First delete all the handling sound and whatever else, so that we just have the noise. Select it, copy it, and then paste it into our original project.

This sound is going to be a reference for the noise reduction algorithm.


### Normalization

However, first we're going to run normalization.

"Edit → Select All" (or Command-A)
"Effect → Normalize": "Normalize stereo tracks independently" should be OFF

What this does is scale everything up so that the loudest portion is at the maximum amplitude. This is important so that you use the maximum bits you have available when you change your audio. Also that the scale of your audio is aligned with other sounds and the volume controls in general, so you're not turning everything up to hear quiet sounds.


### Noise reduction

For step 1, make sure our noise is selected, and then choose "Effect → Noise Reduction..." The click "Get Noise Profile", and click OK. We've now loaded in a "profile" of the noise that will be filtered out.

For step 2, select the rest of the audio with "Edit → Select All" (or Command-A). Choose "Effect → Noise Reduction..." again. Now we can set some parameters:
- noise reduction (dB) is the amount [12]
- sensitivity is how close the match has to be to be considered noise [5.00]
- frequency smoothing (bands) is how it handles any glitches [6]


### Equalization

Select all your audio "Edit → Select All" (or Command-A)

Choose "Effect → Filter Curve"

You'll see a graph similar to what we saw when we learned about the loudness curve of the human ear, and about how all microphones have their own frequency responses.

What we can do here is adjust the overall balance of the audio by raising and lowering frequencies. This is a powerful tool, and small changes can make a big difference, you'll want to make adjustments of just 6dB or less.


## Exporting

Choose "File → Export → Export as WAV" and select "Signed 24-bit PCM". Be sure to rename your file as something descriptive.
