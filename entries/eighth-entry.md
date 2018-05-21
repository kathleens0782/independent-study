# Entry 8: Continuing the Project (Part 3)

With the project's deadline closing in, I've been more ambitious to add finishing touches to my project. I managed to get a lot more of the song done.

Here's the code currently:

```
from earsketch import *

init()
setTempo(120)
track = RD_ROCK_POPELECTRICBASS_20
beat1 = "000+-+000+-+"

for measure in range(1,17):
    makeBeat(track, 8, measure, beat1)
    
for measure in range(5,17):
  fitMedia(OS_OPENHAT01,1, measure + 0.9, measure + 1)
  fitMedia(OS_CLOSEDHAT01,2, measure + 0.01, measure + 0.9)
  setEffect(1, FILTER, FILTER_FREQ, 3000.0)
  setEffect(2, FILTER, FILTER_FREQ, 3000.0)
  
fitMedia(OS_KICK06,3,9,17)
setEffect(3, VOLUME, GAIN, -4.0)
fitMedia(RD_ROCK_POPLEADSTRUM_GUITAR_9,4,13,34)
setEffect(4, VOLUME, GAIN, -8.0)
fitMedia(RD_ROCK_POPELECTRICBASS_20,5,18,34)
setEffect(5, VOLUME, GAIN, 4.0)
fitMedia(RD_ROCK_POPRHYTHM_FILL_3,6,17,18)
fitMedia(Y01_CRASH_1,7,18,18.5)
fitMedia(RD_ROCK_POPRHYTHM_MAINDRUMS_5,6,18,34)
fitMedia(RD_ROCK_POPELECTRICBASS_7,9,35,51)
fitMedia(RD_ROCK_POPLEADSTRUM_GUITAR_10,10,35,51)
setEffect(10, VOLUME, GAIN, -8.0)
setEffect(9, VOLUME, GAIN, 4.0)
fitMedia(RD_ROCK_POPELECTRICBASS_20,12,43,51)
setEffect(12, VOLUME, GAIN, 4.0)
fitMedia(OS_KICK06,11,34,51)

finish()
```
So far, my main goal has been to finish the ending of this song. I haven't decided how I want this song to end, but I hope I think of something. 

As for new changes in the song, there's this:

```
fitMedia(RD_ROCK_POPLEADSTRUM_GUITAR_10,10,35,51)
setEffect(10, VOLUME, GAIN, -8.0)
setEffect(9, VOLUME, GAIN, 4.0)
fitMedia(OS_KICK06,11,39,51)
```
This code will expand into the "B" part of this song's "A-B-A" format. It sounds similar to the first part of the song, but the tracks used are different.

Another way I made sure to get that same familiarity was changing the intro a bit.

```
fitMedia(OS_KICK06,3,9,17)
setEffect(3, VOLUME, GAIN, -4.0)
fitMedia(RD_ROCK_POPLEADSTRUM_GUITAR_9,4,13,34)
setEffect(4, VOLUME, GAIN, -8.0)
fitMedia(RD_ROCK_POPELECTRICBASS_20,5,18,34)
setEffect(5, VOLUME, GAIN, 4.0)
```
The intro uses the same kick sound effect as the one in the previous ccode snippet. This "A-B-A" format is used a lot in many songs; it interests the listener.

### Conclusion

Always assume that your project can have something new added to it; it might give you a great idea. Keep thinking up ideas. If the project is finished, find a way to implement the ideas you come up with later on. 


