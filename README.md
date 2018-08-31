# 7stagesofnaming
An accelerated learning game based on Arlo Belshee's "refactoring is naming" model. This is a "fluency first" game, focused on producing ability, not necessarily understanding or puzzling ability. You are doing the game right if you are doing simple, easy, obvious things, over and over and over. See Llewellyn Falco's "Sparrow Decks" for another example of this.

# The Rules

Sit a group of people down (or a single person) in a coding dojo format (timed rotation with one person at the keyboard), with an IDE open to a chunk of code under test. You have 3 minutes to transition as many blocks of code from a single chosen stage to next. Run tests frequently to make sure you haven't broken anything. When the timer goes off, revert the code and start over for the next person.

Your first time playing the 7 Stages of Naming Game, one stage (such as Missing to Nonsense) will likely fill up the entire hour or so of your coding dojo. Get really good at one stage before moving on to playing with the next - aim for fluency!

# Missing to Nonsense

1. Look for blocks of code, unnammed primitives (strings, numbers, etc), that can be extracted out and given a nonsense name (foo, banana, outgrabeMomerath, etc) that stands out as nonsense. 

2. Only transition the obvious. If you spend more than 10 seconds thinking about it, move on to something else more obvious. The goal is fluency, not puzzling out your options. Do a simple easy thing over and over and over until the timer dings.

3. Run tests to make sure you haven't broken anything. When the timer goes off, revert the code and start over for the next person. Once you've got the hang of Missing to Nonsense, after a full round or three or five, don't revert the last bit of code. You'll build on it for the next stage.

# Nonsense to Honest

1. Looking at all the Nonsense names that you just created, find one that you can easily say one obvious and honest thing that it does. Don't try to sum it up! Just say one honest thing that it does (or is, in the case of a primitive).

2. Transition as many Nonsense names as possible, keeping in mind that the goal is not to puzzle anything out (don't take more than 30 seconds to pick a name - that is a looooong time for this exercise). Just do a simple easy thing, over and over and over until the timer dings.

3. Secondarily, there are named blocks of code that were already in the code - scan those to see if you can rename any of them to say one Honest thing about what the code does or is, if they don't already.

4. Run tests to make sure you haven't broken anything. When the timer goes off, revert the code and start over for the next person. Once you've got the hang of Nonsense to Honest, after a full round or three or five, don't revert the last bit of code. You'll build on it for the next stage.

# Honest to Honest and Complete

1. Looking at all the Honest names, now scan them for an additional Honest thing that they do. Previously, you just picked one of the Honest things that they do, and this likely left a lot of the functionality out. Now add one more Honest thing. If before you named a block of code "convertCurrency" (noting that it also did some formatting for presentation in the UI), add one more thing by renaming it "convertCurrencyAndFormatForUI", for example. NamesCanGetLongerAndLongerAndLongerAndThatIsOK! It's actually very important that long names stand out, just like the Nonsense names needed to scan as true nonsense. It reminds us that there is still more work to do, which will come in the next stage.

2. Follow the same instructions as before in past steps.

# Honest and Complete to Does the Right Thing

1. Now take as many long names as possible and look for opportunities to extract and encapuslate responsiblities that don't fit. Of all the Honest things in the name, does one of them stand out as being (cue Sesame Street song) "One of these things is not like the others, one of these things just isn't the same". Extract it out and encapsulate it.

2. Follow the same instructions as before in past steps.

# More to Come

Watch this space!


