So, you have decided to embark on the journey of *le sing* and you want it to sound good. Great, because I'm about to drown you in audio knowledge.

# What is audio?

It does not matter. What matters is that others can hear it. For that, you need to know every step on the path the audio travels from you to others, because at every point of it the audio can be changed, disappeared or made worse.

# The path

## Sound origin

![image](https://github.com/Algoinde/Audio/assets/10269970/780e6701-9f58-41cd-b095-ae544e0c92b7)

You, the one who speaks or sings. In order for the device to hear you to send the signal along, it needs to have a microphone. Phones already have one built in (so they can phone), but if you are using a computer, you need to buy a mic.

Be mindful of everything *other* than you in the vicinity of the microphone. Everything that you can hear, the mic probably can, too, even the echo off the walls and the hum of a fridge or AC.

## Microphones

Which one to get? I'll give you a short tierlist of microphones you can use.

### Garbage:
* The built-in microphone of your laptop.
* Anything Bluetooth (headphones, headset, etc).
* Not having a microphone.

### Acceptable:
* Your phone mic.
* A mic on a cheap headset (<$20).
* The dingy thing on your earbuds wire.

### Good:
* Wired headset with a quality mic. It will usually cost no less than $50.
* A USB mic on a desk stand. Good ones start from, at minimum, $40.

### Better:
* A USB mic on a mic arm.

### Absolute peak:
* An XLR-connected mic on a mic arm, plugged into a USB audio interface. This will cost you in the vicinity of $150 - $200.

Here's some reasoning behind this ranking.

The laptop mics are usually designed for phone calls and are far away from you, plus laptop manafacturers will pour a lot of noise cancelling on top of these, making the audio sound distant and mushy.

![image](https://github.com/Algoinde/Audio/assets/10269970/4730ada3-47ac-461d-9057-bd0c6f2e1800)

Bluetooth will introduce lots of delay, plus the audio quality of the Bluetooth channel itself is awful in headset mode.

Phone mics are pretty good, but it will be hard to use them for anything other than voice calls off the phone itself.

USB mics are usually fine, but the cheap ones will sound extra bad because the manafacturer has to cram the mic *and* the digital audio converter into one small package. There is also a limit how good headset mics can be, and you can't control their distance from the mouth well.

XLR mic + DAC is *the* professional setup which ensures no quality loss at any point in the chain, but it's an expensive one. XLR is the name of the connector/cable for the mic, and DAC is digital audio converter, aka audio interface. It converts the electrical signals of your mic into something the computer can read.

![image](https://github.com/Algoinde/Audio/assets/10269970/663c9fd0-04b8-451a-ab84-4a73eddd8e47)

> [!NOTE]
> You really don't need to jump into the most expensive option. Grab what you have, even your cheap headset, and proceed with it - the key here is gaining experience in setting this all up so you can swap to something better with ease later.

## What you plug it into

This will depend on the mic setup you've chosen.

If it's like this, it will go into your headset jack.

![image](https://github.com/Algoinde/Audio/assets/10269970/fa7285ee-a0cf-4a13-af6e-3f6782b00dcf)

Some PCs may not have a headset jack, but they will have a separate mic and headphone jack. In this case, you will also need a splitter cable like this.

![image](https://github.com/Algoinde/Audio/assets/10269970/9eeb7a29-aa36-470c-bef2-f7559eb386c8)


If you have a USB mic, it will go into a USB port (and in some rare cases, may require you to install driver software from the manafacturers' website).

If you have an XLR mic, it will go into a USB audio interface with an XLR cable, which will then go into a USB port. The audio interface will also probably require a driver installation.

![image](https://github.com/Algoinde/Audio/assets/10269970/1c5e863c-69b1-4d75-be72-1efb760c7c2d)

Depending on the type of XLR mic you have, it may require +48V power from your audio interface (also called phantom power). Please check if your mic needs it and if your audio interface can provide it, and ONLY turn it on with the mics that need it (can be found in the mic manual). As a rule of thumb, condenser mics need it, dynamic and membrane mics don't (I'll explain the sound difference between those later).

Also, your headphones will then go in the audio interface as well. They may need a plug adapter from smol headphone jack to the big one.You can also plug your speakers into it, requiring another type of audio cable.

## The software side

Let's discuss the next step in the chain of sound. Once you've plugged in your stuff, you need to check it's actually working.

This is where things start to get annoying. You've already spent the money, now we start spending braincells.

### Windows: The system sound settings

You need to open the Sound Settings Panel (the old one (the good one)) in Windows. Press Win+R, type `mmsys.cpl` and press Enter. You can also get to it by typing "Change system sounds" in the Start menu search.

In the "Playback" tab it will show you all the devices that are able to take the sound produced inside the computer and then blast it into the real world (headphones, speakers, the display and so on).

![image](https://github.com/Algoinde/Audio/assets/10269970/830f55a4-d31e-40df-9c27-01fd1e230f80)

In the "Recording" tab it will show you all the devices that can take the sound from somewhere (usually the real world) and bring it into the computer (microphones).

![image](https://github.com/Algoinde/Audio/assets/10269970/5f1882e8-b954-4a84-b950-1269ccf4a6ac)

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

### Inputs and outputs?

It can get confusing with "playback", "recording", inputs, outputs, sources and destinations, especially when different programs call it different things.

Let's define all of them properly.

You have a microphone. For the computer, that's an **audio source**. The audio information is created in the mic by capturing your voice, sent over the wire and the computer receives it.

To receive the signal, the computer needs an **audio input**. That's your microphone/headset jack in the computer, audio comes in here. Once plugged in, it will show up in the computer as **input device**. You're speaking into it, it sends sounds to the computer. From the point of view of the computer, that's input. Same as your keyboard - it is an *input device*.

The confusing thing about it is that an *audio source* can also be running on your computer - for example, a music player app. It's also an audio source, but it's "inside". What is inside can come out, though - so you select an **output device** to play your sound. It is connected to the **audio output** of your computer (headphone jack, for example).

If it's a headset, it will have both input and output in the same jack. Sound input will come from the mic on the headset and sound output will go to your headphones.

In the settings window above, Playback will show *output devices* - audio-making programs will send sound to these. Recording will show *input devices* - audio-listening programs will take sound from them.

### Choosing devices per-application

What you just did in the section above was setting the *default* input or output. Programs can choose to not respect this default and you can pick different devices for different programs.

There's two ways to do this. The first one is in the system itself:

![image](https://github.com/Algoinde/Audio/assets/10269970/605564c8-c613-4687-a585-189c4aa3fd0e)

Right click your audio icon and go to Volume mixer.

![image](https://github.com/Algoinde/Audio/assets/10269970/c522a0ec-34ad-455a-9c02-62f51cd60362)

In the top "System" section will be your default-chosen devices (this part is pretty much the same as the window we opened before, but it's new and clunky).

In the "Apps" below you will see all applications that are outputting sound at the moment. Click on any of them and choose a device for them to use - easy! Don't forget you may need to restart playback or the app for it to realize the output had been changed.

The second way is to set this up in the app itself. Some apps have audio settings and allow you to select what device to use - in Discord, for example, you need to go to Settings -> Voice & Video and select them there.  

> [!NOTE]
> Once more: "Input device" inside applications usually means "this is what I will get sound from", and "Output device" means "this is what I will send sound to".

### Voicemeeter

There are many, many ways to go about mixing your audio, but the easiest one would be to use [Voicemeeter](https://vb-audio.com/Voicemeeter/index.htm). It will allow you to:

* Grab your mic audio
* Grab your PC's sound
* Send audio to whatever you need to (Discord, etc).

The main purpose of Voicemeeter is to mix and route multiple audio sources, as well as creating a handy virtual audio device that will act as a fake speaker - it will take sound from your programs but instead of playing it, it will grab the audio and put it into Voicemeeter. It's called Voicemeeter VAIO (virtual audio input-output).

> [!NOTE]
> In Playback, it will be called `Voicemeeter Input`. Why? From the point of view of Voicemeeter, that is indeed input. For other applications though, it sits at their output.
> 
> Same goes for Recording tab, where it will be called `Voicemeeter Output`. It is the overall output of Voicemeeter, but from the point of view of other programs, it will be their input.

[ ... ]  
Player setup  
Ear Trumpet  
Discord setup  
Effects  
ASIO  
Mac OS  


