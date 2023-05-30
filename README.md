# Mixer Lib

MixerLib is a library that automatically mixes music together.

## Method

MixerLib accomplishes this goal by combining the instrumental of one song with the acapella of another.

Both the instrumental and the acapella are ran through the following steps:

1. Detect the BPM of the songs
2. Stretch both songs to a tempo in-between the two
3. Detect the key of the songs
4. Pitch both songs to a key in the middle

Then the songs are summed into the same audio and the output audio buffer is available through the lib API.