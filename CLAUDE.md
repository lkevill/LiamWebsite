# Liam's personal website

## Who I am
Senior at Cal Poly SLO, economics and business. Spent this summer at AlphaSights
in New York, connecting private equity firms with the experts who could actually
answer their questions. My argument, and the spine of this site: it's who you
know, not what you know — anyone can learn anything, so the scarce thing is
access, not knowledge.

## What this site is
The whole site is my college house living room, drawn in flat vector shapes.
You're sitting on the couch looking at the TV. Objects in the room are clickable;
each one opens a panel that slides up from the bottom.

It has three jobs at once: get me interviews, be the thing I point people to, and
be a creative outlet. The personality is the professional differentiator, not a
distraction from it.

## Reference points
- juliaalvarenga.com — the interactivity and the commitment to one metaphor
- sentennial.org — the content depth and the "currently" page that proves the
  site is alive

## The room
Clickable: fridge (left), window (behind the TV), TV with app tiles, tower
speakers (right), surfboard, basketball, and on the coffee table exactly two
things — a camera with a cord (photos) and a journal with a pencil (writing).

Scenery, deliberately NOT clickable: brick hearth, wood paneling, wainscot,
floor, coffee table, the cable running down from the TV. If everything is
interactive, nothing reads as a place.

Cut on purpose, don't add back without asking: street signs, golf clubs, cooler,
shelf clutter.

## Design rules
- Warm honey wood daylight is the default. `body.night` is the same room after
  the "turn the lights off" toggle. Every new color needs a value in both.
- All color lives in CSS variables at the top of the file. `--ball` (basketball
  orange) is the accent and tints panel borders and section labels.
- Fonts: Bricolage Grotesque (display), Karla (body), Space Mono (small labels).
- Minimal and sharp, with room for one or two playful moves. Restraint is what
  makes the playful part land. Don't animate everything.
- Everything must work on a phone, be keyboard navigable, and respect
  prefers-reduced-motion. The text index below the room is the accessible
  fallback for the whole site — keep it in sync with the room.

## File structure
One file: `index.html`. Inside it, top to bottom — CSS variables, styles, the
masthead, the room as inline SVG, the fallback index, the panel markup, and then
a `CONTENT` object in the script holding every panel's copy. Content changes only
ever touch `CONTENT`. Adding an object means one `CONTENT` entry, one SVG group,
and one line in the fallback index.

## How I want to work
I have basically no coding experience, so:
- Explain what you changed in plain English, and why it worked.
- One change at a time so I can look at it before the next one.
- If I describe a feeling ("the right side looks empty"), diagnose it yourself
  rather than asking me for CSS.
- Tell me when I'm asking for something that will look bad or break on mobile.
- Commit to git after anything that works, so I can always get back.
