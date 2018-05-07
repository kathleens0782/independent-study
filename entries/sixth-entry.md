# Entry 6: Continuing the Project
---
The past week had been a rather productive one for my project. I picked out samples that could work out for the song I'm making.

It was this week that made me think about _what_ kind of rock music I was making. Since their were so many subgenres to this genre alone, I thought that a punk rock/grunge-esque would be fun to make; and I settled on just that as I progressed with this project.

I even kept a list of possible samples within the code to see what I could use in the future:

```
#Guitars:
# RD_ROCK_POPLEADSTRUM_GUITAR_9
# RD_ROCK_POPLEADSTRUM_GUITAR_10
#Bass:
# RD_ROCK_POPELECTRICBASS_7
# RD_ROCK_POPELECTRICBASS_20
# RD_ROCK_POPELECTRICBASS_17
```

And as for the actual code, I started working on what I think the song could sound like:

```
from earsketch import *

init()
setTempo(120)
track = RD_ROCK_POPELECTRICBASS_20
beat1 = "000+-+000+-+"

for measure in range(5,17):
    makeBeat(track, 8, measure, beat1)
    
for measure in range(1,17):
  fitMedia(OS_OPENHAT01,1, measure + 0.9, measure + 1)
  fitMedia(OS_CLOSEDHAT01,2, measure + 0.01, measure + 0.9)
  setEffect(1, FILTER, FILTER_FREQ, 3000.0)
  setEffect(2, FILTER, FILTER_FREQ, 3000.0)
  
fitMedia(RD_ROCK_POPLEADSTRUM_GUITAR_9,4,9,26)
setEffect(4, VOLUME, GAIN, -9.0)
# fitMedia(RD_ROCK_POPELECTRICBASS_20,5,17,18)
fitMedia(RD_ROCK_POPELECTRICBASS_20,3,18,26)
fitMedia(RD_ROCK_POPRHYTHM_FILL_3,6,17,18)
fitMedia(Y01_CRASH_1,7,18,18.5)
# fitMedia(RD_ROCK_POPLEADSTRUM_GUITAR_9,4,18,26)
fitMedia(RD_ROCK_POPRHYTHM_MAINDRUMS_5,6,18,26)
  
# # fitMedia(,3,9,17)
# setEffect(3, VOLUME, GAIN, -2.0)
# # setEffect(3, DISTORTION, DISTO_GAIN, 25.0)
# fitMedia(RD_ROCK_POPELECTRICBASS_2,4,5,17)
# setEffect(4, VOLUME, GAIN, 5.0)

finish()
```

The code is all over the place, but I plan to organize it in the future.

In the meantime, one thing I had trouble setting up was this part:

```
track = RD_ROCK_POPELECTRICBASS_20
beat1 = "000+-+000+-+"

for measure in range(5,17):
    makeBeat(track, 8, measure, beat1)
```

`for measure in range` is still a concept that I'm getting used to, as I tend to get tons of errors while using it and me not understanding why. 

### Conclusion
---
There will be times where you're still adjusting to a code's function, and learning these functions can be harder than you thought. Still,, if that's the case, either google what it does to remind yourself, or experiment with it enough to the point that you feel comftorable using it.