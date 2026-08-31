# What Am AI Really?

## Structure

- Intro
  - Clarifying what arguments I am not making
  - Assuming the technology cannot go away given the existence and viability of local models
- The nature of AI
  - What it looks like
  - The Chinese Room
  - What it is - Artifice
- What can AI actually do
  - The nature of art
  - HITL
  - Code
- My recommendations and my use going forwards

As a technically minded engineer, I feel to a degree *responsible* for informing people on how tech really works
and what is really happening. AI as a technology is facinating. It exists as a bizarre cross section of computer
science, business and energy infrastructure. Not many people properly understand it, what it is truly capable of
and what it is not. The result has been a combination of sycophantic worship and compulsive rejection. Whilst I
am more in favour of the latter, it's not really the whole picture and in general comes from the same place as
the latter. Both come from a misplaced belief in AIs abilities.

Now just to get this out of the way I am not going to talk about the environmental impacts. Whilst these are
significant, individual use is negligible in the larger scheme of the industry. The environmental harm is coming
from the race between these companies to produce better models not individual prompts. These companies are not
trying to find real workable applications of the tech -- they are trying to make a more profitable product. My
focus here is more on AI literacy; giving you a framework of what it is and isn't so that you can make a more
informed choice about how to interact with it. Higher AI literacy is also shown to reduce AI use.

## How Does AI Work?

What we currently call AI is actually serveral neural networks in a trenchcoat. This is why all these AI models
seem to have vast capabilities because they are several specialised parts sharing the load. Neural networks
themselves are pretty damn clever. It is essentially a way of making a computer program itself by giving it a
set of inputs and the expected output for those inputs, the infamous training data. The neural network code then
creates a series of nodes, steps between the input and output, that mimic neurons in the human brain. More nodes
means a more sophisticated AI.

Large Language Models (LLMs) are just neural networks trained on lots of written material and given the task of
filling in the blanks. The ability for them to generate new text is sort of a biproduct of this autocomplete.
LLM platforms just frame the text given to the model as a conversation. Image generating AIs do a similar trick
where they are instead trained to remove noise from an image. Give them an image that's all noise and instead
they make something new. Well sort of new. If you give AI the exact same input (including the same seed for
randomisation) it produces the same output. It is after all a computer.

## What Can AI Do?

This brings us to a slightly more philosophical question of what is it actually capable of. From first glance it
seems more than capable of doing research, making art and writing code. From experience we also know that these
are actually a bit off. Information is made up, the art falls into a very particular bland style and the code is
often not quite right. The mistake is believing that the computer is thinking. Mistaking the artifice for true
intelligence.

John Searle's Chinese Room thought experiment is a great illustration of what is going on. Imagine John is in a
room with a big book, some paper and pens, and two slots in the wall. Through one of the slots John receives
messages written in Chinese. The book contains instructions that John follows precisely to construct a perfect
response to the message in perfect Chinese, which he puts through the second slot. The question here is, does
John now know Chinese? Does the book? Does the room? No, it merely creates the illusion, the artifice if you
will, of writing Chinese. AI does the same with thinking.

Now this illusion is impressive. The fact that we have to call out specific stylistic choices like the use of
semi-colons to identify AI writing speaks to how lifelike it is. But there are trends. This is because at the
training data level there will be trends; the neural network is there to find those trends. It is essentially an
average, a really advanced average. This isn't the whole story obviously, as now these things can search the
internet and take in new data, and summarise or whatever, but that is the broad strokes.

## What Should It Be Used For?

Herein lies the rub. Obviously it shouldn't be used for creative work. We've all seen something written or
illustrated by AI that looks like total crap. A lot of its creative use is completely careless. AI lacks the
human element that makes creativity possible after all. Give two people the same prompt and you will get two
different results as their brains connect the unconnectable, half-remember something they like or just pull
something out of the ether. Two AIs will give you almost the exact same thing, as they are incapable of making
the leaps required to make something new. In this sense AI art will never replace human made art. Anyone truly
interested in art will feel the deep unease with AI art even if efforts are made to hide the usual tells.

Yet I can't help but think that someone must be able to make something from these tools. Please humor me with
this hypothetical. Imagine you are an artist drawing a weekly manga. You want to put backgrounds in your manga,
but it is time consuming and takes away time from working on the foreground, the bits people are actually
looking at. The background is extra. Some manga artists filter photos to use for the background, but you can't
seem to make it gel with your style. So instead you get all your the backgrounds you ever drew previously and
feed them into a locally run AI model to produce new backgrounds for you in your style from your data.

Now I haven't seen anyone actually do this, it requires effort and technical knowledge the average AI "artist"
doesn't have. I don't even know if it would work but I am sure that the additional effort put into the process
would produce something better than pure generative AI. This is because instead of treating AI as intelligent
something capable of creation you are treating it as a work horse. Getting it to do what is essentially busy
work. That is, as far as I have experienced, all AI is truly good for. It cannot by its very nature do true
creative work, but it sure as hell can churn out busy work.

I have used AI to code, in a process termed agentic coding. It's basically a more guided form of vibe coding
with the AI editing files on your computer under your direct supervision. The model I used was DeepSeek running
on my own hardware (so not using a datacenter) and let me tell you I understood the appeal. Instead of the usual
programming process of figuring out what to do at a high level and then having to muddle my way through Googling
how to do it in Python again I could just tell the AI to follow my high level plan. It got stuff wrong, sure,
but hot damn was it faster than I would have been. The AI was able to quickly and decisively cut through the
busy work of programming. This is incredible in the hands of someone who knows what they are doing, and is able
to intervene and adjust as the machine does the basics.

The interesting thing about this approach to coding is how it plays the sycophantic nature of AI against itself.
AI should be writing, you are the editor. Instead of asking the model to give you feedback and getting back
some form of praise or softened criticism, you are telling the AI where it messed up. You identify and, if
necessary fix mistakes. Now the AI's eager-to-please tone is more like a diligent employee than the first member
of your cult of personality. Theoretically this approach is also hardened against AI psychosis as you are not
requesting validation from the machine -- though the only true defense there is your mental health.

For all my praises though I would only ever do this again sparingly. I still have a lot to learn programming
wise and a tool like this would enable me to make a lot of high powered mistakes. It is dangerous in the hands
of people without the knowledge to check the outputs. AI can't keep the big picture in "mind" so it often makes
mistakes when not guided specifically enough. This is why vibe coded software is such a mess, there is no
thought put into how each piece interacts with each other. Again this is because it can only pretend to think.
It is artificial. A lie. A simulation.

If you are going to use AI I have some recommendations. First never treat it like a person. It has no opinions
and no ideas. This is not a thinking machine, it is a machine that follows a series of steps that look like
thinking. Second is to always check the output. Anything you get from the machine should be read and verified
with human eyes. It is not a person, it will not feel bad when you fix its work or when you send it back. Third
is to run it yourself. If it's not on your machine its not your data and if you are not paying for it you are
the product. For most normal uses the current models can be run on anything with 32GB of RAM. Finally, never
offload your thinking to a machine. AI is a powerful tool if it is treated as a tool and not a machine god.
