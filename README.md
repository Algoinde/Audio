So, you have decided to embark on the journey of *le sing* and you want it to sound good. Great, because I'm about to drown you in audio knowledge.

## What is audio?

It does not matter. What matters is that others can hear it. For that, you need to know every step on the path the audio travels from you to others, because at every point of it the audio can be changed, disappeared or made worse.

## The path

### Sound origin

You, the one who speaks or sings. In order for the device to hear you to send the signal along, it needs to have a microphone. Phones already have one built in (so they can phone), but if you are using a computer, you need to buy a mic.

Be mindful of everything *other* than you in the vicinity of the microphone. Everything that you can hear, the mic probably can, too, even the echo off the walls and the hum of a fridge or AC.

### Microphones

Which one to get? I'll give you a short tierlist of microphones you can use.

#### Garbage:
* The built-in microphone of your laptop.
* Anything Bluetooth (headphones, headset, etc).
* Not having a microphone.

#### Acceptable:
* Your phone mic.
* A mic on a cheap headset (<$20).
* The dingy thing on your earbuds wire.

#### Good:
* Wired headset with a quality mic. It will usually cost no less than $50.
* A USB mic on a desk stand. Good ones start from, at minimum, $40.

#### Better:
* A USB mic on a mic arm.

#### Absolute peak:
* An XLR-connected mic on a mic arm, plugged into a USB audio interface. This will cost you in the vicinity of $150 - $200.

Here's some reasoning behind this ranking.

The laptop mics are usually designed for phone calls and are far away from you, plus laptop manafacturers will pour a lot of noise cancelling on top of these, making the audio sound distant and mushy.

Bluetooth will introduce lots of delay, plus the audio quality of the Bluetooth channel itself is awful in headset mode.

Phone mics are pretty good, but it will be hard to use them for anything other than voice calls off the phone itself.

USB mics are usually fine, but the cheap ones will sound extra bad because the manafacturer has to cram the mic *and* the digital audio converter into one small package. There is also a limit how good headset mics can be, and you can't control their distance from the mouth well.

XLR mic + DAC is *the* professional setup which ensures no quality loss at any point in the chain, but it's an expensive one. XLR is the name of the connector/cable for the mic, and DAC is digital audio converter, aka audio interface. It converts the electrical signals of your mic into something the computer can read.

### What you plug it into

This will depend on the mic setup you've chosen.

If it's like this, it will go into your headset jack.

[pic]

Some PCs may not have a headset jack, but they will have a separate mic and headphone jack. In this case, you will also need a splitter cable like this.

[pic]

If you have a USB mic, it will go into a USB port (and in some rare cases, may require you to install driver software from the manafacturers' website).

[pic]

If you have an XLR mic, it will go into a USB audio interface with an XLR cable, which will then go into a USB port. The audio interface will also probably require a driver installation.

[pic]

Depending on the type of XLR mic you have, it may require +48V power from your audio interface (also called phantom power). Please check if your mic needs it and if your audio interface can provide it, and ONLY turn it on with the mics that need it (can be found in the mic manual). As a rule of thumb, condenser mics need it, dynamic and membrane mics don't (I'll explain the sound difference between those later).

Also, your headphones will then go in the audio interface as well. They may need a plug adapter from smol headphone jack to the big one.You can also plug your speakers into it, requiring another type of audio cable.

### The software side

Let's discuss the next step in the chain of sound. Once you've plugged in your stuff, you need to check it's actually working.

This is where things start to get annoying. You've already spent the money, now we start spending braincells.

#### Linux

Good luck. You got this.

#### Windows

##### The system sound settings

You need to open the Sound Settings Panel (the old one (the good one)) in Windows. Press Win+R, type `mmsys.cpl` and press Enter. You can also get to it by typing "Change system sounds" in the Start menu search.

In the "Playback" tab it will show you all the devices that are able to take the sound produced inside the computer and then blast it into the real world (headphones, speakers, the display and so on).

In the "Recording" tab it will show you all the devices that can take the sound from somewhere (usually the real world) and bring it into the computer (microphones).

What the names and icons are will depend entirely on your PC and what you have plugged in. You'll have to use common sense and experimentation to figure out what device represents what. Play some music and see what Playback devices' level meter is moving. You can change between them by right-clicking and selecting "Set as default device" - the one that is default will have a green checkmark on it.

If the meter is bouncing but you don't hear anything, see on the device itself if it has any volume knobs to turn it up.

In the Recording tab, get real close to your mic or tap on it *lightly* and see what's moving. It will make sure you don't have your laptop mic selected by accident.

Once you've found the correct devices and figured out what their names are (remember them for later!), you're halfway there.

> [!IMPORTANT]  
> Changing, connecting or disconnecting audio devices can make things hiccup or stop. You may need to restart playback, restart the audio player, restart Discord (full-quit it from the taskbar in the bottom right) and so on.

> [!TIP]  
> Go into *all* your devices' properties, both playback and recording ones, by double-clicking them. On the Advanced tab, disable everything in "Exclusive mode". This will prevent programs wrestling over the device and causing hard-to-figure-out debauchery. Some games may not like this though, so if you run into issues down the line we'll turn it back on.
>
> While you're there, disable all "Enhancements" too, if there are any. We can bring them back later, but you should always start with a clean signal.

##### Voicemeeter

There are many, many ways to go about mixing your audio, but the easiest one would be to use [Voicemeeter](https://vb-audio.com/Voicemeeter/index.htm). It will allow you to:

* Grab your mic audio
* Grab your PC's sound
* Send audio to whatever you need to (Discord, etc).

The main purpose of Voicemeeter is to mix and route multiple audio sources, as well as creating a handy virtual audio device that will act as a fake speaker - it will take sound from your programs but instead of playing it, it will grab the audio and put it into Voicemeeter. It's called Voicemeeter VAIO (virtual audio input-output).

There's also a "fake microphone" part of it, which will take the mixed audio from Voicemeeter and show up as a microphone in your programs - this is how you send the mixed audio to Discord, for example.




