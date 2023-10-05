---
layout: post
title:  Some things that do not work with ZMK firmware
date:   2023-10-04 22:37:31
categories:
 - keyboard
 - ZMK
 - kinesis
---

This list was compiled by ~~painstaking research~~ haphazardly dorking around
with ZMK firmware while trying to program a Kinesis Advantage 360 Pro.  With any
luck, by the time you read this most of the bugs will be fixed.  Maybe even some
of the features that I want will exist.  And Santa Claus will have come to town.
With.Presents.

Well I fantasize a lot.  Which should be apparent by the fact that I'm trying to
program a Kinesis keyboard to do what I want, rather than what it wants.

A lot of my frustration deals with coming from QMK for an Ergodox Infinity that
I used for quite some years.  That gave me enough time to become quite
comfortable with it.  So naturally, everything I do is going to be judged in the
light of how great QMK is (ok, so that was a fantasy too, but one I liked).

On to the complaining.  First of all, ZMK does not have mouse movement keys.
That was a real bummer, because it was crucial to me being able to give up the
mouse.  Now the mouse is back on the desk, looking at me with its one good eye.
Some crazy programmer out there has a branch where it works.  And it's only a
hundred commits behind the current branch of ZMK.  Selah.

I almost cried when it was time to give up the HYPER, MEH and META keys.  ZMK
has META, but it's just mapped to Windows key alias.  I really miss HYPER and
MEH for leader keys in Linux and Vim.  They can be programmed as modifier keys
to other keystrokes, but not mapped directly to a physical key.

Then there's the rather useless hold-tap keys.  The basic idea is that you can get
two different pieces of functionality for a single key by holding it longer.
This allows for modifier keys on the home row keys. I got really excited when I saw
some of the other keyboard modders out there with homerow mods.  Wow! Then I 
figured out why nobody was using homerow mods.  The timeout for the hold key was
way too short.  I was creating rollover misses like crazy.  There's a 
super-complicated-to-the-point-of-crying fix for that from a user called urob,
but you have to dedicate a significant portion of your life to it.

Then there was the idea that layers were going to make a virtually infinite
number of keys available.  That kinda went out the window when the hold-tap keys
didn't work.  That is, there would have to be modifier keys on the default layer
to access all of those other layers.  Since the hold-tap doesn't really work,
there are only about 6~8 keys really available to change layers, depending on
your default layer programming.  

There is a way to combine keys for combined activation, but there is no way to 
access that while still using the GUI configuration tool.  This also goes for
tap-dance and custom hold-tap settings.  If you want precise control, at some
point you will outgrow the GUI, and that point comes sooner than you think.

There may come a time when my configuration is stable enough that I don't need
the GUI configuration tool any more.  At that point, there will be a one-way
abandonment of the tool in favor of further customizations.  Flexibility vs.
convenience.  You pick, but you can only pick once.

There is also a difference that I'm having a bit of a hard time quantifying.  I
have the RIGHT\_GUI mapped to the keyboard.  For some reason, Ubuntu doesn't
want to recognize it in combination with other keys for shortcuts.  It shows
hitting the key as RIGHT\_META, but then won't register the second combined
keystroke.  Not sure why that's so, but it is very annoying.

All that being said, I was able to port about 95% of the QMK configuration to
ZMK.  The stuff that was missing was ultimately not critical to function,
although it did require some brain remapping.

Even though the HYPER and MEH keys were missing, I just mapped different keys
there and then changed the Linux compose key to those.  My fingers don't know that
they're not hitting different key codes, so I guess that's good enough.

I didn't find a reasonable-human way around the hold-tap behavior.  That's ok,
because QMK didn't have that anyway.  Nothing in my current setup depended on
it.  Oh, well.

Overall, the migration went smoothly.  The Kinesis has already become my daily
driver, and the Ergodox is all but forgotten.  Although these shortcomings are
kinda important, they ultimately didn't become showstoppers.  In a future blog
post, I'll talk more about the new features that make ZMK a bit easier to use
than QMK was.  Stay tuned.
