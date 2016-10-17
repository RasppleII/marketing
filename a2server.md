# a2server.svg, "Your Files Are Served"

Created by T. Joseph Carter

While the a2cloud project is hard to define, a2server is pretty easy: It's
AppleTalk for older computers via an old version of netatalk.  Sure, we throw
Samba in there, and we use ciopfs (case-insensitive on purpose filesystem) to
make it ProDOS 8 friendly while retaining expected GSOS and Mac behavior, but
it effectively comes down to being about the AppleTalk.

I rather like the flat cell-shaded look of the graphics on the Raspberry Pi
website, and it's no secret I've been a fan of flat cell-shaded graphics since
I was probably about three.  😃  I thought I would model the a2server icon on
the AppleShare icon Apple used in the IIgs and early Macs, but that wasn't
going to work without an icon.

I had other things to work on at the time, so I reached out to [Raspple II
Central][] on Facebook and asked if someone could vectorize the AppleShare
icon as SVG.  Didn't expect I could use the result legitimately, but maybe I
could get some quick inspiration?

That's when Michal Lutinsky and Charles Ottman stepped up.  Charles took the
original icon and, as far as I can tell, used the trace bitmap feature of
Inkscape on it.  This was a little too rounded, but it had the kind of
cartoony charm I wanted.  Michal actually took a screenshot of a larger mono
drawing of the hand/tray/icons and removed the background.

I didn't want to try and reproduce anything like the larger hand because I
didn't think it could look good, but that simple change Michal had made kinda
did, and Charles had caught the flavor I wanted.  I knew what to do then.

The tray and icons on it were mostly easy.  The folder, app diamond, and
document page icons were just lines after all.  I actually made the app
diamond not quite a true diamond by flatening the tips.  You won't see that
unless you render it at high resolution, but the lack of sharp points was a
touch inspired by Charles' rounded version.

The app icon's hand...  I could have carefully calculated curves, but I
didn't.  😉  Yes, at long last, I actually have drawn a graphic without even
primarily the use of a text editor.  All my friends from the quake modding
days would be shocked, I'm sure.  The XML is still done by hand, mostly
because Inkscape's SVG output is still a steaming heap, but if I'm starting to
understand how to use editing tools and it speeds the process, why not?

Yeah, I'd actually learned some stuff between this and The Raspple, so what I
did was draw a polygon with Inkscape, copied the `d` attribute into my
hand-edited SVG file, and fixed the coordinates which were not where I wanted
them.  Then I opened that back up and used the node tools to curve the lines
into the shape you see.  Cleaned up the `d` in Inkscape's built-in XML editor
(for instant visual feedback) and copied it into my by-hand SVG file.

That left the large hand holding the tray.  Fortunately, in the process of
doing the app icon, I'd learned how to do it!  Polygon it out to create
vertices and endpoints for curves, adjust them with precision in XML, and use
the node tool.  Held up my own right hand and looked at it side-on for drawing
the polygons.  I'm left-handed (like all the great geniuses of history) so it
was easy to hold my hand as I modeled it on the canvas.  I looked like a dork
I'm sure, and my pinky is too short.

Believe it or not, the hardest part of modeling the hand shapes was recreating
an effect Charles probably obtained by pure accident.  I would've left (and
did leave on the app diamond) the hand fill as a hard corner at the cuff.  I
realized though at the cale I was dealing with on screen, having a curve there
gave it a shadow.  I could leave the corner square, but I didn't want to, and
by not doing so the outline fill creates a shadow effect.  Very happy with
that.

The hand details were drawn as thin polygons, cleaned up, autocurved, slightly
edited, then cleaned up again.  By this time a familiar process, if not
exactly a simple and automatic one.

As I write this, I've just finished giving it some color and I'm pleased with
it.  You might notice two different skin tones used for the hands.  The big
hand--the one modeled on my own?  That's got a normal skin tone.  The hand
holding the pen in the app icon is clearly an albino, however.  😎

[Raspple II Central]: https://www.facebook.com/groups/rasppleii/

