Tracker Thoughts
================

This is not a software project, but a temporary sketch repository.

Two years ago, I made github.com/mpdehaan/camp, which was a generative music
project based in Python.

Unfortunately the language got to be too declarative and weird, kind of like a semi-modular synthesizer setup for creating MIDI events.

What I really want to do is write my *own* music with it, and to do so, making a computer music tracker is compelling.

What follows in this repo are several examples, with the idea that the project this tool would consume would be directories.

This is all subject to change but I wanted to get some feedback.

Configuration
=============

Every song is a directory or repo.

There is a score file which contains some globals like bpm but mostly things are set with directives in the patterns themselves

Score file
==========

The score file basically describes the composition in a micro-language.

See example/score for an example of what this may look like.

Here we can define drum tracks that don't get affected by the current scale.

We can also define sections of music and then repeat those sections.

MIDI file
=========

This defines the track mappings.

See example/midi for what this may look like.

It will define the midi channels for each named track and also maybe some names
for import MIDI CC controls.

Pattern files
=============

Pattern files live in the patterns.d directory. I have included some examples but they are basic.

The number of notes per bar defaults to 16 if not set.

Expressions like "C4 for 4" means to hold a C4 for 4 sixteenth notes.

Questions
=========

Is this good or bad?  How can it be improved?

CAMP as a project has code to do nearly all of this easily, it just needs to be reworked some once the language gets sorted out.



