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

- Importing of square, hex and gridless maps
- Basic character sheet creation via plain text markup files that become
interactive forms in the UI
- Dice rolling with robust syntax
- Basic macro system that can interact with character stats
- Simple and manual fog of war system that snaps to the map grid

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
