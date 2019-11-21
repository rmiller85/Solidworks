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

![alt_text](https://github.com/rmiller85/Solidworks/blob/master/Screenshots/gear.JPG "Sorry about the cropping. It's abominable.")

So I had my gears. Now for the "box" part of Gearbox. First, I had to make the frame that our gears would be attatched to. I got a picture, displayed below, of what our basic dimensions should look like. 

![alt_text](https://github.com/rmiller85/Solidworks/blob/master/Screenshots/frame_ideal.PNG "Perfect!")

Under that, I had directions on what a few dimensions were and a tip on how far apart the holes should be. From there, it was sink or swim. I...didn't swim. Not once, not twice, not four times, but *three times* I deleted all the shit I had made for the frame and started over. Finally, on my third attempt, I picked up an idea from some other people: instead of trying to 
