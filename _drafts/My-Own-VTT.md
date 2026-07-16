# Making My Own VTT

The way I see it indie RPGs/the OSR need their own easily modifiable
universally adopted VTT. Something everyone can use and tailor to
their games, without the work and licensing required of something more
complicated like Foundry. As much as I love it Foundry is quite bloated.

I think a lot could be achieved with a VTT that acts as a simple framework
that handles the map, whilst providing tools for things like dice
rolling and character sheets. Then anything custom is stored as a combo
of markup files, YAML data files, images, and scripts making them
portable. Imagine if a map maker could give you a little YAML config
file with the PNG that aligns it to the grid perfectly first time. This
would be a godsend to most online GMs.

## Minimum Viable Product

This is the basic stuff I want out of a VTT. It is a little more than
some minimalist offerings like Owlbear Rodeo, but I think handling character
sheets in a shared environment helps more than it hinders (especially
if handled right). It is just a small piece of mental load that doesn't
need to be placed on anyone at the table.

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
