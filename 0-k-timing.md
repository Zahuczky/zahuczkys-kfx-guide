
# Aegisub K-Timing Guide
So, you’ve chosen to learn the ways of k-timing songs inside Aegisub.  
Sit back and relax, this is going to be easy.

## Our workspace
![enter image description here](https://files.catbox.moe/t7q1yb.png)

> *Audio Panel Inside Aegisub*


Let’s quickly go through what you can find in the audio panel.  
The three sliders to the right control vertical and horizontal zoom on your audio visualization, and volume. Go ahead and play with them a bit.

Inside your visualizer, you can see three distinct “lines”, a red, white and blue one.  
The red line is the start time of your line.  
The blue line is the end time of your line.  
The white is the current position of your playback cursor.

There’s also a plethora of buttons under the visualizer, let’s quickly go through all of them.



 
|||
|--|--|
|<img src="https://zahuczky.com/wp-content/uploads/2022/05/Aegisub9215_2kWeBhVmXi-1.png" alt="drawing" width="200"/> |With these two buttons, you can switch between your lines|
|<img src="https://zahuczky.com/wp-content/uploads/2022/05/Aegisub9215_SHS0L3pBKN-1.png" alt="drawing" width="200"/>|The blue button plays through all of your lines selected in the subtitle grid, while the red only plays the currently active line.|
|<img src="https://zahuczky.com/wp-content/uploads/2022/05/Aegisub9215_NhG41EXcDb-1.png" alt="drawing" width="200"/>|This is pretty self explanatory, but for the sake of completeness, this button stops playback.|
|<img src="https://zahuczky.com/wp-content/uploads/2022/05/Aegisub9215_2EyOmYDMdd-1.png" alt="drawing" width="400"/> |These four buttons will be good friends of yours for timing songs. They play a bit before your line, a bit after your line, a bit after the start of your line, and a bit before the end of your line, respectively. With these you can make sure your timing is always on spot, and never bleeds.|
|![enter image description here](https://zahuczky.com/wp-content/uploads/2022/05/Aegisub9215_pHyUkklj5s-1.png)|With these buttons you can add lead in/out times to your lines. Not useful for us, only for dialogue timers.|
|![enter image description here](https://zahuczky.com/wp-content/uploads/2022/05/Aegisub9215_zc4YDhBXDz-1.png)|The green check icon commits all recent changes to your line, the blue arrow scrolls to the center of your audio selection. Not too useful for us.|
|![enter image description here](https://zahuczky.com/wp-content/uploads/2022/05/Aegisub9215_SkTTtMI864-1.png)|These are our main settings. In respective order, they auto-save all of our changes to the line(so we don’t need to manually press the button mentioned above), automatically go the next line on committing changes(k-timers should turn on automatic saving, so this is irrelevant), scroll the visualizer when we play back the video/click around in the grid, switch between the modes of the visualizer(for k-timing, you wanna use this mode), the last one is some sort of legacy key binding mode, for the predecessor of Aegisub, Medusa.|
|![enter image description here](https://zahuczky.com/wp-content/uploads/2022/05/Aegisub9215_G79ECD84MC-1.png)|Our best friend. Toggles between line timing/k-timing mode.|
## Timing lines
First and foremost, you need to time the lines properly, before even thinking about doing any karaoke timing.

Basically there’s only one rule we have to follow when we’re timing the lyrics that are going to be kfx-d.  
**Never leave empty space at the beginning/end of your line!**

In practice:

![enter image description here](https://files.catbox.moe/mlklz2.png)
In this image, we can clearly see in the visualizer, and hear that the first syllable of our line starts where my cursor is pointing.

So don’t do this:

![enter image description here](https://files.catbox.moe/6au3i5.png)

Do this instead:

![enter image description here](https://files.catbox.moe/pttsdk.png)
Apply the same principles to the end of the line. If you feel like there is room for a buffer, you want the line to stay on-screen a bit longer, don’t worry, that’s the job of the kfx-er. They’ll add the necessary lead in/out time in the effect templates.
|  ![enter image description here](https://zahuczky.com/wp-content/uploads/2022/05/Aegisub9215_2EyOmYDMdd-1.png)|You can use these buttons to check if it’s actually correct.|
|--|--|

## K-Timing
Now, let’s get down to business.  
With the button mentioned above, switch to karaoke mode.

![enter image description here](https://files.catbox.moe/5prf08.png)

You can see that our panel changed a bit. Our words are visible in the visualizer, there are some yellow lines in between them, and a new strip appeared with our lyrics, with some blue lines in between.

Let’s talk about that new strip first.  
That’s where you can divide your lyrics into syllables, by clicking between the letters.

![enter image description here](https://zahuczky.com/wp-content/uploads/2022/05/splitsyls.gif)
> Kinda like this.

Don’t forget to press the green commit button after you split your syllables.

Now, the yellow lines represent the start/end times of our syllables.  
We can start sliding them around, and with that, actually k-timing our song.

The MOST IMPORTANT buttons during this part, are SPACE and the LEFT/RIGHT arrow keys. By pressing space, you can listen to the active syllable, and with the arrow keys you can jump between them, with playback.  
Always listen to the syllable multiple times, and also listen to a bit before and after the syllables with the buttons mentioned above, to make sure it doesn’t bleed over to the next.

![enter image description here](https://files.catbox.moe/f2yb8f.png)
> The visualizer is a big help to time perfectly.

If you turned auto-saving on(you should), your changes are already in the line. Playing back the video, you’ll see your timed line, with the color of the line changing between your first and secondary colors.

The last thing we have to pay attention to, is that sometimes there is a break between some of our syllables.

![enter image description here](https://files.catbox.moe/nxs39y.png)

We have two ways to deal with them.  
We can add an empty syllable there, just by clicking again between those syllables in the strip we used before. This is what we  **_should_** do for long and significant break.

![enter image description here](https://files.catbox.moe/7tok2d.png)
> Like this

Or in cases where that break is _really_ short, we can add them to the syllable before.

![enter image description here](https://files.catbox.moe/f2yb8f.png)

What we have to pay attention to, is to never add those breaks to the beginning of a syllable. Our syllables should always start where they actually do in the audio.

I think that’s kinda it.

~Have fun
