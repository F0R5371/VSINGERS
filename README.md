# VSingers
Welcome to the VSingers repository, a place where all information about virtual singers and related topics can be found.

## Voicebanks
Voice banks simply refer to a sound library that virtual singers are created on.

They are the foundations of a virtual singer and without them there would be no voice to synthesize. 

There are mostly two main types of file types that come with a voicebank:
- wav files : the actual recordings of the singer whose voice will be synthesized
- frq files : frequency files corresponding to each wav file used by the resampler

As well as those two main types of files, often things like character icons (icon.bmp), descriptions (character.txt and readme.txt)

However, one if not the most important file in a voicebank has to be the oto.ini file. Inside this file is all the configuration settings of an Utauloid's voice.

### Voice Configuration (oto.ini explained)
The oto.ini file is largely responsible for how each wav file and its respective frequencies are processed. 

While all of the parameters and numbers of the oto.ini may seem overwhelming and confusing at first, they really aren't too complicated once you see how everything works together.
These values may be different based on the type of voice bank as well but more on that later.

The main parameters of the oto.ini are as follows:
- alias : another name for the wav file being processed
- set : path of the wav file 
- file : the actual name of the wav file
- phonetic : typically represents the character/letter voiced in the wav (often times, however, the phonetic and alias are just the same)

- offset (start of audio): where the sound will actually start playing
- overlap (green line): the overlap determines roughly where a note prior to this specific note will fade to
- preutterance (red line): simply defined as where the note starts, this has different interpretations for vowels and consonants, more on that later
- consonant (pink region): covers the critical parts of the sound, as well as before the vowel actually starts
- cutoff (end of audio): where the sound stops playing


