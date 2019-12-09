# Solidworks
Pictures and descriptions of my Solidworks assignments. This is intended to ~~get me a good grade~~ be used as a tool for other people doing these assignments, providing an overview of my experience, with some helpful advice scattered around.

## Design Tables
In this assignment, we made a design table which would provide a bunch of configurations for a spool. This would make it wider, have more screw holes, etc. It's pretty basic. One thing I had a bit of trouble with was accidentally jacking up the configurations because I didn't set changes to `This configuration` as opposed to `All configurations`. Dumb mistake, still happened though. Here's a picture of the various spool sizes, lined up.

![alt_text](https://github.com/rmiller85/Solidworks/blob/master/Screenshots/design_tables_spool.png "Here it is!")

## Advanced and Mechanical Mates
For this, we had to make this weird little thing.

![alt_text](https://github.com/rmiller85/Solidworks/blob/master/Screenshots/adv_mate_pic.png "I don't have the foggiest as to what this is")

The twist: it had to be able to extend, controlled by sliding the little pin in the middle. That wasn't a great way of describing it, so here's a picture. Warning: this picture is the epitome of comedy if you have the mind of a 3rd grader.

![alt_text](https://github.com/rmiller85/Solidworks/blob/master/Screenshots/adv_mate_pic_extended.png "e x t e n d e d")

I had to make the three rectangle things and add configurations of them so that they fit together all nicely. I didn't have any issues with this ~~except when I was hecking stupid and forgot to turn off all configurations *again*~~. I then had to make the pin. Nothing really to say about that; I just put in the measurements given to me.

Now, for the interesting part. Up until now, I had never delved into the realm of what I called "wack mates". Remarkably eloquent, I know. But for this, we had to use `Width`, `Linear/Linear Coupler`, `Slot`, and `Tangent` mates (actually, `Tangent` is one of the standard mates, but whatever). The width one was to make the rectangle things inside of each other. From there, I used the linear mate to make them slide in and out of each other together, but at different rates. I then used the slot mate to put the pin inside its slot. Finally, I used a tangent mate to connect the pin to one of the rectangle things. This made it so that sliding one would slide the other. Done!

## Gears and Gearbox

Oh lord. This was a *time*. 

My assignment: first, create gears. Then, create axels, spacers, frames, and a knob. Then assemble all of it and mate it so that the gears all mesh properly. Simple, right? So yeah, it was a lot.

I started by making my gears. I used a design table to make 4 configurations of different sizes. These had a bunch of variables that would change with each configuration. In fact, the different gears were different *because* of these altered variables. Almost all of the dimensions were equations. For example, the radius of each gear was a variable: `addendum_diameter`. Some others were actual equations, though. An example of that would be the size each tooth. the number of teeth was simple: that was stored in the variable `teeth`.  However, the size was `180/"teeth"`. Our instructions were pretty confusing in a few places, but hopefully that will have been addressed by the time whoever reads this is working on that assignment. It was talking about how you need to do this to that construction line, but there's a hundred construction lines, and how "that little line goes to the side arc." (but which one? What line? What even is a gear?) It was a mess. Eventually, I got it to a tolerable level of not-awfulness, and made the extraordinarily wise decision to say that it was good enough. Here's a picture of one of my gears.

![alt_text](https://github.com/rmiller85/Solidworks/blob/master/Screenshots/gear.JPG "Sorry about the cropping. It's *abominable*.")

So I had my gears. Now for the "box" part of Gearbox. First, I had to make the frame that our gears would be attatched to. I got a picture, displayed below, of what our basic dimensions should look like. 

![alt_text](https://github.com/rmiller85/Solidworks/blob/master/Screenshots/frame_ideal.PNG "Perfect!")

Under that, I had directions on what a few dimensions were and a tip on how far apart the holes should be. From there, it was sink or swim. I...didn't swim. Not once, not twice, not four times, but *three times* I deleted all the stuff I had made for the frame and started over. Finally, on my third attempt, I picked up an idea from some other people: instead of trying to make a bunch of weird arcs, just do rectangles and circles that overlap, then use the `Trim Entities` tool to get it all fixed up. That approach, however, led to this catastrophe.

![alt_text](https://github.com/rmiller85/Solidworks/blob/master/Screenshots/box_frame_withrelations.png "This could literally be the before photo to a before/after")

Disgusting. That said, it was fully defined and fully functional, so I just went with it. I am certain that there is a better way. I just didn't find it.

Anyway, with that done, I made an axel with a short and long configuration. No issues there, just put in the measurements. Then, I made spacers with a handful of configurations for different sizes. Again, no issue. I then made assemblies, putting the gears on axels and putting in spacers. Again, no issues. Then, I had to make a knob. This would theoretically be turned, turning the gears. I had a bit of trouble getting the dimensions to cooperate, but no major issues.

Finally, the assembly. I did all the normal mates to get things attached, then delved into the realm of `Gear` mates. Turns out, having the whole thing kind of assembled made it more confusing to do the gear mates, so I got rid of a bunch of mates, then moved on to the actual gears. The gear mates were kind of wack, but I got it figured out. Finally I could assemble the whole thing and watch the magic!

![alt_text](https://github.com/rmiller85/Solidworks/blob/master/Screenshots/gearbox_shields.JPG "Expectation")

![alt_text](https://github.com/rmiller85/Solidworks/blob/master/Screenshots/gearbox_pic.png "Reality")

## Motion Study

For this assignment, I had to make this weird little mess of parts, assemble it, and make a motion study of it. "What's a mtion study?" I can hear you asking. Well, I could very well be wrong on this, but I'm pretty sure the best way to desrcibe it is this: a simulation of how your assembly will react to movement. I made a bunch of parts according to measurements I was given, assembled them without any issues, and did the motion study according to the instructions. This ran into some issues, however. I was getting a weird error that I didn't understand: `Dynamic simulation stopped due to incompatible redundant constraints present in the system.` I didn't have the foggiest as to what that meant. I searched it up and discovered a way to make the redundant mates automatically become a bushing. I'm not quite sure what a bushing is, but whatever. It was a complete disaster. Mr. H tried to help me, but in the end, he decided to take pity on me and just let me be done. Here's a picture of the god-forsaken thing.

![alt_text](https://github.com/rmiller85/Solidworks/blob/master/Screenshots/motionstudysshot.png "Finally done, I guess.")

## Stress Analysis

This was a pretty cool one. I really got to see the practical uses of Solidworks. We had to make a part and run some tests on it. I made the part without issues and pulled up `SimulationXpress Analysis Wizard`. Note: I'm pretty sure you have to turn off `Solidworks Simulation` in Add-Ins. From here, the instructions were pretty easy to follow except for one thing: it says to select the face of the large hole. This means to select the inside of the cylinder, not the top of it. I know that was an atrocious way to explain it, so here's a picture of my part with the face that you want to select highlighted.

![alt_text](https://github.com/rmiller85/Solidworks/blob/master/Screenshots/stress_analysis_pic.png "Trust me, it's all worth it to see the animation.")

Ok, so it's time to see the animation now. Solidworks senses where the part could move and *wiggles* it. Honestly I don't know why it looks so funny to me. I guess I just never aged past 11.  At this point, the instructions asked me to make the part stronger. I tried making the hole in the middle smaller. This worked relatively well, but, thanks to Harrison, I discovered that there was a *far* bette way to strenghthen it. Make the cut in the middle leave a slice in the middle as a support. This *dramatically* improved the strength of the part.
