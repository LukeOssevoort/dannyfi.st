# Making My Own VTT

The way I see it indie RPGs/the OSR need their own easily modifiable
universally adopted VTT. Something everyone can use and tailor to
their games, without the work and licensing required of something more
complicated like Foundry. As much as I love it Foundry is quite bloated.
The ideal is something that is default simple, but can be made more
complicated.

## Minimum Viable Product

This is the basic stuff I want out of a VTT. It is a little more than
some minimalist offerings like Owlbear Rodeo, but I think handling character
sheets in a shared environment helps more than it hinders (especially
if handled right). It is just a small piece of mental load that doesn't
need to be placed on anyone at the table. The goal is to allow basic
systems to be implemented by the average user (ie character sheets and
basic dice roll automation) with no plugins or modifications. 

### Maps

The obvious part is allowing for square, hex and gridless maps that you
can plop tokens onto. Where I think just a little bit of extra effort
would help is allowing map makers to package their image with some data.
Instead of maps just being a `png` or `jpg` they could also include a small
[YAML][yaml] file specifying the grid type, size and offset so that
everything is aligned on import. Package them in their own zip file with
a special file extension (like `cbz` for comics) and you have something
easily sharable for creators and usable for players.

Map visibility should be handled by a simple, manually controlled fog
of war system. Automatic vision looks flashy but in practice it breaks
constantly and behaves unexpectedly. It ruins reveals, dungeon crawling
and flow at the table. It is much easier if the GM can just pick what
tiles are visible.

### Character Sheets

This is another area where I think should be dead simple and be a big
improvement on existing VTTs. Basic principle is that character sheet
templates should be easily creatable in a markup language, even just
markdown with some use specific syntax. Then you can describe stats and
macro buttons in sheets that are easily sharable and automatically conform
to the VTT's look and feel. This makes implementing new or niche systems
easy too.

### Dice rolling

Dice rolling syntax is already pretty will defined in other apps. So I
think the rub here is in the specifics. Variables like stats should be
easy to reference, defaulting to pulling from whoever made the roll.
So instead of referring to `self.mods.dex` it would be just `dex` making
it easier for most users to make a simple macro for common rolls.

## Wishlist features

With the list above, you would have a pretty solid VTT that would do
just about everything you truly *need*, so now let's talk about wants.

### Layers

The best feature of Roll20 is the layers. As a GM it means you can hide
tokens ahead of time only to reveal them all at once, put notes on the
damn map and do basic overlay effects. It's great and it could be better.
Imagine having complete control over what layers are available and
their visibility. You could have one GM layer just for notes, one for
ambushes and have multiple player layers to handle different elevations.
Way more elegant than more advanced systems and easily understood by
new users.

### Map building

Basically inbuilt tools for sketching out a map or dragging it together
from tiles. Think Dungeon Scrawl or HexKit, except integrating into the
map specific zip file idea from earlier. So now you can build and export
a map in a zip file that either includes all the assets, or if you can't
redistribute the assets references them in a redistributable way. You
could even use a different tile set.

### Styling

Chances are the styling of the app will be handled by CSS, so why not
let the users modify it. CSS as a technology would allow the layering
of styling. There can be a style defined for the system that could then
be overwritten by the users to their preferences. It also means those
with colour blindness, dyslexia or any other disability that might limit
accessibility can style their client to suit their needs.

### Visual Scripting

Not everyone knows how to code, and lack the sufficient blend of motivation
and probable autism to do so. These people still need macros, so what
are they to do when the macro they need does not already exist. This
is where visual scripting comes in. Everyone understands a flow chart.
So instead of typing, users can assemble their macros out of predefined
operations that can be linked together in a flow chart.

For example here is a basic 5e roll:

```mermaid
flowchart TD
  A[1d20] --> C{==20?}
  C -->|True| D[Output Critical Success!]
  C -->|False| E{==1?}
  E -->|True| F[Output Critical Fail]
  E -->|False| B(+STR)
  B --> G[Output roll value]
```

and here is a Cairn roll:

```mermaid
flowchart TD
  A{Advantage/Disadvantage?} -->|No| B[1d20]
  A -->|Advantage| C[Lowest 1 of 2d20]
  A -->|Disadvantage| D[Highest 1 of 2d20]
  B --> E{<=STR?}
  C --> E
  D --> E
  E -->|True| F[Success]
  E -->|False| G[Failure]
```

### A Standalone App

The real issue with any of the DIY VTT solutions is you have to learn
how to host a server. Hell my Foundry setup uses Docker containers! No
normal person should have to learn containerisation. Instead it should
just be peer to peer more or less. Unlike multiplayer video games, TTRPGs
don't really incentivise cheating so why are we making tools that act
like they do? Players should just be able to run up the app, share a
code and start playing.

Additionally, I like single use tools. This trend of trying to be more
intentional by switching from the nightmare rectangles in our pockets
to a handful of purpose built things is nice. I want it to extend to
the digital gaming table as much as possible and that means getting
out of the web browser. It is way too easy to get distracted when you
are basically playing next to the open sewer of the internet.

### Plugins

I think the ideal of a tool like this is having a low barrier to entry
but the ability to make things more complicated as needed. *Lancer*
players would likely love some rules automation, but many systems can
do without for example. Now this feature would basically make this VTT
Foundry but with a simpler starting point (and FOSS). Which I guess is
the point I was making the entire time.

[yaml]: https://yaml.org/about/
