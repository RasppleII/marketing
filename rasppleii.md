
# rasppleii.svg, "The Raspple"

Created by T. Joseph Carter

This is the story of one man's bold quest to fix it later.  :D

The first thing you need to know is that I hate what Inkscape spits out for
SVG files.  The XML is largely write-only, and it strangely mixes relative and
absolute coordinates.  It's a mess, I don't like it, and I'm not very
proficient with it anyway.  It helps that I have some background in OpenGL
graphics and a long history of drawing XPM graphis by hand using the trusty
vim text editor.  :)  Those of you who know that I'm legally blind can
probably appreciate my amusement at the look on people's faces when I tell
them these things.

This image started with graph paper, a circle template, and me "eyeballing"
the December 2012 Raspberry Pi logo [found on Wikipedia][rpi-logo].  The graph
paper helped me quickly type the circles into the SVG file, but the end result
was just an outline lacking the leaves from the original.  My fiancee told me
it looked more like grapes than a raspberry.  It did--I'd fix it later.

I joined all the circles into a single path in Inkscape and used the XML
editor to grab the "d" of the path to put into my hand-made file.  I split the
path nodes up for easier reading and reloaded the file to make sure it still
worked.  Then I set about tweaking the XML bit by bit with a calculator to
stretch the circles out and make the result look more raspberry-ish.  This
worked, but I had to recalculate almost every single node by hand.  Slowww!
But like I said, no proficiency with Inkscape, so I didn't know how to do it
right.

Then I dropped white circles on top of it and again turned these into paths I
could stretch and reshape as above.  It was at this point I tried to reduce
precision on the nodes of the "berry bits" to reduce filesize.  Introduced
some flaws this way, but you only saw them at high res, and at this point I
still needed just a tiny icon for GitHub--I'd fix it later.

It was then I discovered two problems:

1. Despite trying to make something inspired by, but obviously not the RPi
   logo, by removing the "grapiness" I'd all but recreated their logo without
   the leaf in black and white.
2. The leaf was necessary, and all my attempts to draw one had failed.

Given the first problem was already an issue, I cheated to solve the second:
Loaded the RPi logo and zoomed in on the leaves at the bottom of the screen
and superimposed a grid.  On the top, I opened the XML file and started
writing a path object by hand using linetos to make a sawtooth leaf fill.
Opened that in Inkscape and of course it looked terrible.  Solved by new
understanding of the smoothing tools!  But now it looked even more like the
RPi logo--I'd fix it later.

I decided to solve this by carving a chunk out of the berry and painting it
with the colors of the 1970s rainbow Apple Computer logo.  Using one company's
former trade tress to help me avoid infringing another company's current trade
dress.  What was I thinking?  Except that the result would be a nice homage to
both companies for a project that bridges their products.

The color looked great with a mod to the leaves, except I didn't have any
desire to re-calculate all of those nodes to modify the paths just then--I'd
fix it later.

I showed what I had to the #a2c.chat IRC channel and Tony Diaz reacted to my
proud work simply by saying, "Take a bite out of it!"  Craaaaaaap.

I did that eventually, and while I was working on the logo for a2server I
learned enough Inkscape tricks to actually clean it up to be the image you see
now.  And that's when I decided it should go into version control.

The result is the file you see here.

[rpf-logo]: https://en.wikipedia.org/wiki/File:Raspberry_Pi_Logo.svg
