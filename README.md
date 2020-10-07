# 7 Stages of Naming
An accelerated learning game based on Arlo Belshee's "Code by Refactoring" model. This is a "fluency first" game, focused on producing ability-to-do-under-pressure, not necessarily high-level understanding or puzzling ability. You are doing the game right if you are doing simple, easy, obvious things, over and over and over (of course, finding easy, obvious things to do isn't as easy as it sounds...) See Llewellyn Falco's "Sparrow Decks" for another example of this (http://llewellynfalco.blogspot.com/p/sparrow-decks.html).

# The Rules

Sit a group of people down (or a single person) in a coding dojo format (timed rotation with one person at the keyboard), with an IDE open to a chunk of code under test. The person at the keyboard is the Driver, their job is to implement the ideas of the group. They have 3 minutes to follow group instructions to transition as many blocks of code from a single chosen stage to next. Run tests frequently to make sure you haven't broken anything. When the timer goes off, keep the code changes and build on them for the next person.

Your first time playing the 7 Stages of Naming Game, one stage (such as Missing to Nonsense) will likely fill up the entire hour or so of your coding dojo. Get really good at one stage before moving on to playing with the next - aim for fluency!

# Missing to Nonsense

1. Look for blocks of code, that seem to "hang together". For example, a few statements that start with a comment, and have a blank line after. `Extract Method` on a block and give a name of _obvious nonsense_ (foo, banana, outgrabeMomerath, etc). Also look for unnamed primitives (strings, numbers, etc) that can be extracted as a variable or constant.

2. Only transition the obvious examples. If it takes you more than 10 seconds of thinking, move on to something else more obvious. The goal is fluency, not puzzling out your options. Do a simple easy thing over and over and over until the timer dings.

3. Run tests after every refactoring/renaming to make sure you haven't broken anything. When the timer goes off, keep the code changes and build on them for the next person. Once you've got the hang of *Missing to Nonsense*, or when you can't find any more transitions to make, after a full round or three or five, you can move on to the next stage.

# Nonsense to Honest

1. Looking at all the Nonsense names that you just created, find one that you can easily say one obvious and honest thing that it does. Don't try to sum it up! Just say one honest thing that it does (or is, in the case of a primitive). If a block of code checks for errors and returns data, just pick one of those - either the errors (checkForError) or the data (returnData). Don't try to sum both up in one concept. This will be important later. **Once again: DO NOT SUM UP! Pick one aspect of the code you've given a nonsense name, and put a name to that. That's all. Leave the rest alone even if it could easily be summed up. There lies dragons! It will break this step if you sum up.** Pull the different aspects apart. Be picky! Pick one Honest thing out of all the things it does or is, and give that thing a name.

2. Transition as many Nonsense names as possible, keeping in mind that the goal is not to puzzle anything out (don't take more than 30 seconds to pick a name - that is a looooong time for this exercise). Just do a simple easy thing, over and over and over until the timer dings.

3. Secondarily, there are named blocks of code that were already in the code - scan those to see if you can rename any of them to say one Honest thing about what the code does or is, if they don't already.

4. Run tests to make sure you haven't broken anything. When the timer goes off, keep the code changes and build on them for the next person. Once you've got the hang of Nonsense to Honest, or when you can't find any more transitions to make. You'll build on it for the next stage.

*Feel free to also use previous stages that you've become fluent at in a more advanced session. For example, if you're currently focused on Nonsense to Honest, and you see some Missing names that stand out, go ahead and transition them to Nonsense, and then move on to your next transition to Honest.*


# Honest to Honest and Complete

1. Looking at all the Honest names, now scan them for an additional Honest thing that they do. Previously, you just picked one of the Honest things that they do, and this likely left a lot of the functionality out. Now add one more Honest thing. If before you named a block of code "convertCurrency" (noting that it also did some formatting for presentation in the UI), add one more thing by renaming it "convertCurrencyAndFormatJsonForUI", for example. NamesCanGetLongerAndLongerAndLongerAndThatIsOK! It's actually very important that long names stand out, just like the Nonsense names needed to scan as true nonsense. It reminds us that there is still more work to do, which will come in the next stage.

2. Follow the same instructions as before in past steps.

*Feel free to also use previous stages that you've become fluent at in a more advanced naming stage. Go ahead and transition any obvious Missing or Nonsense names to the next higher stage.*

# Honest and Complete to Does the Right Thing

1. Now take as many long names as possible and look for opportunities to extract and encapuslate responsiblities that don't fit. Of all the Honest things in the name, does one of them stand out as being (cue Sesame Street song) "One of these things is not like the others, one of these things just isn't the same". Remove it from the Honest and Complete name and extract it out and have it called separately, or encapsulate it. Now the Honest and Complete name is shorter! Use these overlong names to signal mixed and overly coupled responsibilities that you can extract from both the name and code.

2. Follow the same instructions as before in past steps.

# More to Come

Watch this space! Once you feel you've mastered a stage, check out Arlo Belshee's blogposts breaking down each stage and revealing things you may not have though of.

* Missing to Nonsense: http://arlobelshee.com/naming-is-a-process-part-2-missing-to-nonsense/
* Nonsense to Honest: http://arlobelshee.com/naming-is-a-process-part-3-nonsense-to-honest/
* Honest to Honest-and-Complete: http://arlobelshee.com/naming-is-a-process-part-4-honest-to-honest-and-complete/
* Honest-and-Complete to Does the Right Thing: http://arlobelshee.com/naming-is-a-process-part-5-honest-and-complete-to-does-the-right-thing/


