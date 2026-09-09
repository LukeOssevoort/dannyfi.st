# What Am AI Really?

As a technically minded engineer, I feel to a degree *responsible* for informing people on how tech really works
and what is really happening. AI as a technology is fascinating. It exists as a bizarre cross section of computer
science, business and energy infrastructure. Not many people properly understand it, what it is truly capable of
and what it is not. The result has been a combination of sycophantic worship and compulsive rejection. Whilst I
am more in favour of the latter, it's not really the whole picture and in general comes from the same place as
the former. Both come from a misplaced belief in AI's abilities and the perceived inevitability of Artificial General
Intelligence (AGI).

Now just to get this out of the way I am not going to talk about the environmental impacts. Whilst these are
significant, individual use is negligible in the larger scheme of the industry. The environmental harm is coming
from the race between these companies to produce better models not individual prompts. These companies are also not
trying to find real workable applications of the tech -- they are trying to make a more profitable product. Whilst
these conversations are worthwhile my focus here is more on AI literacy; giving you a framework of what it is and
isn't so that you can make a more informed choice about how to interact with it. Higher AI literacy has been shown
to be correlated with a more appropriate conditional trust of the technology[^ai-lit-citation].

## How Does AI Work?

What we currently call AI is actually several neural networks in a trench coat[^neural-nets]. This is why all these
AI models seem to have vast capabilities because they are several specialized parts sharing the load. Neural networks
themselves are pretty clever. It is essentially a way of making a computer program itself by giving it a
set of inputs and the expected output for those inputs, the infamous training data. The neural network code then
creates a series of nodes, steps between the input and output, that mimic neurons in the human brain. More nodes and
better training data means a more sophisticated AI. This is of course a wild oversimplification as the actual
research is not really my field and is progressing so rapidly that anything I do get specific about will be wildly
out-dated.

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
will, of a system that knows Chinese. AI does the same with thinking, each piece alone is not thinking.

In fact the research really bears out this failure in actual intelligence. When models began to use "reasoning" to
enhance results[^reasoning] Apple conducted research into the actual intelligence of these new reasoning models.
Long story short, in some scenarios the new models failed to outperform the old ones, presented inconsistent logic
in solving the puzzles and demonstrated clear diminishing returns on increased context[^apple-paper]. This is even
a known quantity in the world of agentic coding (vibe coding's more studious cousin) with the so-called "dumb zone"
[^dumb-zone].

Now this illusion is impressive. The fact that we have to call out specific stylistic choices like the use of
semi-colons to identify AI writing speaks to how lifelike it is. But there are trends. This is because at the
training data level there will be trends; the neural network is there to find those trends. It is essentially an
average, a really advanced average. This isn't the whole story obviously; as now these things can search the
internet, take in new data and summarize what it finds. This is just the broad strokes of what these models
are doing.

## What Should It Be Used For?

Herein lies the rub. Obviously it shouldn't be used for creative work. We've all seen something written or
illustrated by AI that looks like total crap. A lot of its creative use is completely careless. AI lacks the
human element that makes creativity possible after all. Give two people the same prompt and you will get two
different results as their brains connect the un-connectable, half-remember something they like or just pull
something out of the ether. Two AIs will give you almost the exact same thing, as they are incapable of making
the leaps required to make something new. In this sense AI art will never replace human made art. Anyone truly
interested in art will feel the deep unease with AI art even if efforts are made to hide the usual tells.

The issue with pure AI output is the complete lack of intention in the creation. Anyone putting out these AI works
is not actually interested in making something, they just want the result. In a way they want the artifice of
creativity with none of the hard work. They do not want to push past the phase of being kind of bad at something
or at the very least below the standards of their taste. This makes AI art really no different to normal bad art;
it's thoughtless. There is no human in the loop.

Yet I can't help but think that someone must be able to make something thoughtful from these tools. Please humor
me with this hypothetical. Imagine you are an artist drawing a weekly manga. You want to put backgrounds in
your manga, but it is time consuming and takes away time from working on the foreground, the bits people are actually
looking at. The background is extra, especially in manga. Some manga artists filter photos to use for the
background, but you can't seem to make it gel with your style. So instead you get all the backgrounds you ever
drew and feed them into a locally run AI model to produce new backgrounds for you in your style from your data.

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
but hot diggity was it faster than I would have been. The AI was able to quickly and decisively cut through the
busy work of programming. This is incredible in the hands of someone who knows what they are doing, and is able
to intervene and adjust as the machine does the basics [^scale].

The interesting thing about this approach to coding is how it plays the sycophantic nature of AI against itself.
AI is writing, you are the editor. Instead of asking the model to give you feedback and getting back
some form of praise or softened criticism, you are telling the AI where it messed up. You identify and, if
necessary, fix mistakes. Now the AI's eager-to-please tone is more like a diligent employee than the first member
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
is to protect your data. If you are working with anything personal or sensitive, like say sorting your
emails, you should be running the model on your own hardware. If it's not on your machine its not your data and
if you are not paying for it you are the product. For most normal uses the current models can be run on anything
with 32GB of RAM. Finally, never offload your thinking to a machine. AI is a powerful tool if it is treated as a
tool and not a machine god.

[^ai-lit-citation]: This study shows overreliance in those with low AI literacy and the need for AI literacy in education [https://arxiv.org/html/2604.01114](https://arxiv.org/html/2604.01114) and this study identifies AI literacy as a key factor in appropriate trust calibration [https://arxiv.org/pdf/2501.10909](https://arxiv.org/pdf/2501.10909).
[^neural-nets]: Neural networks is the bedrock technology at the very least, there has been many changes in how these models are developed and deployed that make this a bit more complicated.
[^reasoning]: Basically a method of making LLMs spell out a thought process before giving an answer resulting in more precise answers
[^apple-paper]: The paper itself is worth a read [https://ml-site.cdn-apple.com/papers/the-illusion-of-thinking.pdf](https://ml-site.cdn-apple.com/papers/the-illusion-of-thinking.pdf)
[^dumb-zone]: This talk by agentic coding advocate Matt Pocock about his methodology starts with an outline of the dumb zone and his steps to combat it [https://youtu.be/-QFHIoCo-Ko?si=Bd31FaqoZ-GfSpe_](https://youtu.be/-QFHIoCo-Ko?si=Bd31FaqoZ-GfSpe_)
[^scale]: It is worth noting that this approach does not scale. An individual being discerning and careful can get a lot done, but extend that to a big team and you have problems. Uber for example burned through its entire AI budget for 2026 in 4 months with no indicators towards its performance [https://fortune.com/2026/05/26/uber-coo-ai-spending-tokens-claude-code/](https://fortune.com/2026/05/26/uber-coo-ai-spending-tokens-claude-code/). Anecdotally, experienced software engineers are finding themselves spending more time fault finding bad AI code from careless juniors thanks to AI increasing their output.
