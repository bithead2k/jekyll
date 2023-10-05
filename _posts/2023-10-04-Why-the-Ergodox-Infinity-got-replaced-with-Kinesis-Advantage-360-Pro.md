---
layout: post
title:  Why the Ergodox Infinity got replaced with Kinesis Advantage 360 Pro
date:   2023-10-04 21:42:01
categories:
  - keyboard
  - kinesis
  - ergoonomic
  - adv360
  - ergodox
---

Well friends, after 6 years of hacking on an Ergodox Infinity, I'm finally
making a switch to a Kinesis Advantage 360 Professional.

That switch is not without some pain and a bit of worry, but it had to be made.

TL;DR:  The Ergodox was finally giving up the ghost.  On my particular keyboard,
the right hand USB-c connector was never soldered correctly, and made a kind of
wachelkontakt (thanks German).  This progressed to holding my mouth correctly
when plugging it in 5 years ago.  Four years ago, it got mounted to the desk so
that the connector wouldn't move.  Well, it actually moved a bit anyway, which
was enough that it finally wore out last week.

I went to quite some heroics to try to fix it.  Unfortunately, the USB-c
connector is soldered into a very inconvenient place underneath the
microcontroller.   To get to the problem, I would have to de-solder all of the
switches (to get the pc board off) and the microcontroller (to get to the connector).   
I just wasn't ready to do that without having a spare on hand.  Except that if I 
had a spare on hand, why would I bother to fix the old one?

After it completely died, I went looking for pc boards.  I thought maybe I could
build a new one and just re-use the old case.  Even if I were willing to order
parts from Asia and wait for them, nobody was selling the board that fits in my
case.  Any replacement kit would effectively be a complete replacement, and I
would lose my LCD screens in the process.

So, I tried to replace it with a retail unit.  An even more unfortunate rabbit hole.  I ordered
this as a kit from MassDrop (yes, you read that right).  That was nearly 7 years
ago, and apparently the first drop was the only one that ever shipped.  AFAICT,
there was never another one like it.

There are a few clones out there, such as the ErgoDox EZ, the HotDox, the
Moonlander and some etsy accounts that will build custom units.

So, maybe it was finally time for something a bit different.  In the mean time,
there are much better Dactyl kits and some miniature keyboards (all the way down
to 8 keys!).  After bingeing on YouTube for a few days, I found the Kinesis
Advantage 360 Pro, and realized that it was effectively a well-made commercial
version of the Ergodox.  What a find!

Now this was a very pleasant surprise for me.  For the first 17 years of
software development, I used a Kinesis Advantage Pro QD.  I'm probably one of
the first 100 customers that Kinesis ever had.  That keyboard was an XT
connector.  I got it in about 1996 or so.   Somewhere around 1998, I put an AT
connector extension on it.  About 2003, I added a USB-A adapter.  In 2015, my
chain of connectors finally failed.  So I bought a new one!  The only difference
from 1996 was that it now had a USB-A connector directly on it.  And that was
the keyboard that I was using when I ordered and built the Ergodox.

The Ergodox is programmed with QMK (yes, I know there are other options).  The
first keyboard layout that I programmed for myself was effectively a copy of the
Kinesis Advantage Pro QD.  All I did was remap a few keys the same way that I
had remapped them on the Kinesis.

Over the course of the 6 years that I used the Ergodox, I made many,many changes
to the QMK layout.  New application specific layers, macros, leader keys, cursor
movement, mouse replacement...  the list goes on.

So, (if you're still reading at this point) you can imagine my joy that Kinesis
had not only created a keyboard with **exactly** the right layout, and **exactly** 
the right tenting, spacing and curvature that I wanted...they had also made it
programmable!  Ok, it was with ZMK, not QMK.  But that should be pretty trivial
to convert.

So, here.  Take.My.Money.  A lot of it. Then charge me shipping. Then make me
buy the keycaps that should have come with it.  Ok, make me buy the wrist rests
also.  I don't care.  I'm a sucker for punishment.  Make me learn a new macro
language to do the same things I've been doing for 25 years.  Come on, Kinesis.
Do me hard.  I can take it.

It took about 5 days to do all the stuff with ZMK that I had previously done
with QMK.  There were some exceptions, though.  A few things that I had to give
up, and a few pleasant surprises.  I did most of that programming in the
7 shipping days before the new keyboard ever showed up at my door.  When it got
there, it only took me another 6 or 7 hours to get everything **actually**
working.

And here I am.  Typing away at my Kinesis Advantage 360 Pro keyboard.  It has
been 2 days since the keyboard was nominally functional for me, and I'm already
running it as a daily driver.  The poor Ergodox is lying punched-out and lifeless
on the floor. Victorious, but now replaced by the new fighter.

Let's hope this new keyboard has the same staying power that the old QD Pro did.
Because it's also laying on the floor right next to the Ergodox, still
functional, but abandoned.

Quo vadis? I don't know.  I tend to stick with a keyboard for quite some years
(as my story attests).  This is likely to be the set of keyboards that I retire
with.  I guess that's the ultimate win for Kinesis.
