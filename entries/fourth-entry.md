# Entry 3: Practicing Loops and Learning Effects
---
For this week, I focused less on learning something and moving on and more of trying to practice with what I've learned so far.

I've started thinking about what kind of song I should make. There's so many genres to choose from after all; picking one will be a little hard.

For now, I've been messing around with loops, such as making stuff like this:

```init()
setTempo(120)

drums = RD_ROCK_POPRHYTHM_MAINDRUMS_2
bass = RD_ROCK_POPELECTRICBASS_1

for measure in range (1, 18):
  fitMedia(drums, 1, measure, measure + 2)
  fitMedia(bass, 1, measure + 0.5, measure + 1)
finish()
```
And I also got around to learning how to add SFX into songs:

```
from earsketch import *

init()
setTempo(180)

fitMedia(HOUSE_ACOUSTIC_PIANO_006,1,1,17)
fitMedia(YG_ELECTRO_PIANO_LOW_1,2,9,17)
setEffect(1, VOLUME, GAIN, 5.0)
setEffect(2, VOLUME, GAIN, 10.0)

finish()
```

### Command Notes ♪♫♬
---
`setEffect()`: Makes SFX and other cool things that can happen in a song (Ex: delays, volume and pitch adjustments, distortions, etc.)

### Conclusion
---
My takeaway from this entry is that while learning new things is a good thing, redoing and practicing with what you already know is even better. Try experimenting: even if you get a bunch of failures at first, you'll get it eventually.