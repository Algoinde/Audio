So, you have decided to embark on the journey of *le sing* and you want it to sound good. Great, because I'm about to drown you in audio knowledge.

# What is audio?

It does not matter. What matters is that others can hear it. For that, you need to know every step on the path the audio travels from you to others, because at every point of it the audio can be changed, disappeared or made worse - so take some time to understand each step on the sound's path so you can be confident that your sound is in your own, knowledgeable hands and you can easily fix it if it breaks.

# The path

## Sound origin

![image](https://github.com/Algoinde/Audio/assets/10269970/780e6701-9f58-41cd-b095-ae544e0c92b7)

You, the one who speaks or sings. In order for the device to hear you to send the signal along, it needs to have a microphone. Phones already have one built in (so they can phone), but if you are using a computer, you need to buy a mic.

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

The main purpose of Voicemeeter is to mix and route multiple audio sources, as well as creating a new output device. Programs can send audio to it but instead of playing it, it will grab the audio and put it into Voicemeeter. It's called Voicemeeter VAIO (virtual audio input-output).

> [!NOTE]
> In Playback, it will be called `Voicemeeter Input`. Why? From the point of view of Voicemeeter, that is indeed input. For other applications though, it sits at their output and it is an *output device*.
> 
> Same goes for Recording tab, where it will be called `Voicemeeter Output`. Voicemeeter will be the *audio source* in this case, and that device is "output of Voicemeeter". But from the point of view of other programs, it will be an *input device*, because they can listen to it.
>
> It's a bit confusing. The naming makes more sense if you read it as "Voicemeeter's Input" and "Voicemeeter's Output". You can even double-click and rename them so it's less confusing.

Let's break down Voicemeeter itself now (I'll call it VM).

![image](https://github.com/Algoinde/Audio/assets/10269970/21a98838-35af-48ad-a860-8b7a8ce4c8da)

Things we need to do here are:
1. Put our microphone inside VM
2. Put our music player inside VM
3. Listen to music *and* the voice in our headphones
4. Send the combined VM audio to Discord

#### 1. Microphone
In the top left, click `1` near "Microphone" to select your Microphone device (remember what it was called?). There will be several copies of the same thing, but they will be "WDM", "KS", "MME" - choose the one with WDM. If it doesn't work, try the MME one. If *that* doesn't work, try the KS one. It's just different ways to grab the audio source.

#### 2. Music player
For this one, you don't need to set anything up in VM. Simply select "Voicemeeter Input" as the output device of your player (in the system [Mixer settings](#choosing-devices-per-application)).

#### 3. Listen to the result
In the right section of VM, you can choose where it will output the sound to. Click on `A1` on the top right and select the device through which you want the music to play. Use the same option (WDM, MME, KS) as the input.

> [!WARNING]
> If you select your speakers, things could become VERY LOUD. Your microphone may start picking up your speakers, and then putting the sound back into speakers again, creating what is known as "feedback loop". **It's better to use headphones**.

Now, there's big `▸A` and `▸B` buttons to the left of each volume slider.

If `▸A` is enabled, it means the sound from that channel will go to the device you've chosen in `A1` just now.

If `▸B` is enabled, the sound will go to `Voicemeeter Output` device that you can use in other apps as input.

So, we want to keep all of these enabled. We want to hear the music and the voice to check that it's all there (`▸A`), and we want all of that to go to Discord, too (`▸B`).

You can disable (`▸A`) on your microphone if you don't want to hear yourself talk, but I usually leave it on at all times.

#### 3a. The issues
Things rarely go like you want them to. Here's what you might encounter:

<details>
  <summary><b>Delay</b> <i>[click to expand]</i></summary>
  
  If there's significant delay between you talking and hearing yourself, try going here:

  ![image](https://github.com/Algoinde/Audio/assets/10269970/abd4ac29-ed06-43e4-b28c-9d7a7b6425fc)
  ![image](https://github.com/Algoinde/Audio/assets/10269970/c8c69731-19d4-48c3-9177-64d3c3a216cb)
  
  Big scary window. We only need to pay attention to two things here. Click on "Buffering WDM" (if that's what you've chosen) and chose 64. Now check that there are a) no errors after that b) the `buf:` thing above says the same number you've chosen (or close to it). If it falls back to 1024 or 512, that means it failed. Click the Buffering button again and select the next number above 64. If that fails again, go for the next highest number until the `buf:` thing shows the correct number. It'll probably be 128 or 256, depends on your system. The lower the better.
  
  This should resolve the delay. If it doesn't, try closing this window and switching everything to MME instead (the mic, the output). After that, return and do the same process with `Buffering MME`.
</details>

//

//

//

[ to write... ]  
Ear Trumpet  
Discord setup  
Effects  
ASIO  
Mac OS  


> Be mindful of everything *other* than you in the vicinity of the microphone. Everything that you can hear, the mic probably can, too, even the echo off the walls and the hum of a fridge or AC.

