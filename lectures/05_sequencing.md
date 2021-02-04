# Sequencing

Once you have cleaned up an audio track, you may want to work with it further. Combining audio clips into new sequences, layering clips on top of each other, and arranging them in space as well as in time are the basic components of composing with sound, whether you are working in a musical context, with documentary or field recordings, or to express your expressive goals as a sound artist.

## Multi-track editing

So far, we have been working with a single stereo "track" of audio. However, Audacity lets us create as many tracks as we want in order to create layers.

Open an audio file in Audacity and save the project as "sequencing_exercise.aup".

Choose "Tracks → Add New → Stereo Track". An empty track will appear below the initial one.

Select some audio, and choose "Edit → Remove Special → Split Cut". This behaves similarly to when we use Split Delete to remove a portion of a clip. However, this time the audio is stored in the clipboard.

Select somewhere on your new track, and choose "Edit → Paste". Your clip will appear on the new track. Use the <-> tool to move it forward and backward in time.

Note that once you create multiple tracks, "Select All" will select your entire project. To just select all the audio on one track, there is a "Select" button on the track controls. To just select a single clip, use the selection tool and double-click on it.

## Amplitude envelopes

Arranging clips on the timeline across different tracks leaves space between them. This is fine, but it also means that the clips start and stop abruptly. In addition, want if we want to control the relative volume of the clips?

As a starting point, the "- +" control on the left side of each track controls the overall volume. You can use this to adjust the whole track at once.

For more fine-tuned control, and in order to create gradual volume transitions, we'll use the envelope tool. By clicking, holding, and dragging up and down on a clip, you can see how the amplitude of the waveform is adjusted. By just clicking once, you'll create a new control point, and either side of that point can be adjusted independently. To remove a control point, simply drag it outside the track.

By crafting envelopes, you aren't limited by the dynamics of your recordings, and you can expressively control how they are presented to the listener.


## Spatialization

If audio on two different tracks overlaps, you will hear them at the same time. However, you don't need to hear them in the space. Amplitude envelopes can create a sense of foreground and background and movement between the two. But we can also control side-to-side positioning and movement in the stereo field.

Just like with volume, we have an overall _pan_ control on the left of the track ("L R"). However, we do not have a panning curve in Audacity.

...but we can simulate one.

To do this, we first have to separate our stereo track into two mono tracks. Do this by clicking on the name of the track and selecting "Split Stereo to Mono". As a result, each channel in the stereo track is now on its own new track.

Using the track controls, pan the top one all the way to the left, and the bottom all the way to the right. This will create the same result as the original stereo track.

However, we can now adjust the envelopes of each side independently. If the audio envelope between the two tracks differs, we will hear the sound move through space. <!-- show extreme fade example -->

Once you're done, select the control area on both of the tracks. You can then select "Make stereo track" by clicking on the name of either one. You will now have a recombined track with stereo movement.


### Reverb

An important aspect of spatialization is the reverberation in the space of the recording. "Reverb" is an effect that simulates this acoustic effect.

Select some audio, choose "Effect → Reverb", and play with the parameters.

In order to make things sound like a real space, you'll want to use Select All to apply the effect to all of the audio. Applying separate reverbs in multiple places will create artificial or distorted senses of space. Of course, if that's what you want, that's fine too.

<!--
bonus: how is analog reverb produced?
(reverb rooms, springs, plates, etc)
-->


## Additional Effects


### Audio rate manipulation

There are a few more additional techniques that mimic what is possible with magnetic tape. The first is changing the playback speed of a track. Click on the track name, and select "Rate"—you'll see a list of standard sample rates, and an option to supply your own.

If you recorded your audio at 48kHz, selecting 16kHz will play back the audio at 1/3 the speed. It will be both slower and lower in pitch. Play around with different track modifications and listen to what they do to the sound.

In addition, there is "Effect → Reverse", which will flip the order of samples in a clip.


### More

By now you have noticed that there are other effects that we haven't talked about. Audacity provides many built-in possibilities, though its options tend to be fairly utilitarian in nature. Commercial "Digital Audio Workstations", or DAWs, like Logic and Protools, will be loaded with advanced effects of all kinds. These are all great, and feel free to explore. Remember, however, the that the techniques we've looked at here (mic placement, splicing, normalization, eq/filter, sequencing, envelopes, spatialization, and reverb) are the foundation, and work with these first to craft your audio intentionally without relying on layers of processing as a crutch.
