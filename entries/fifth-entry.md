# Entry 5: Starting the Project
---
After weeks of practicing Earsketch commands, I finally felt like I could start working on the project.

I will try to see if I can teach myself some more commands, but for now, I wanted to focus on starting my project.

The troubling part was deciding what genre I want to pick. I have many in mind: Rock, Electro/Electro Swing, Funk, Chillwave, Cinematic, etc. I had already decided on making a two or three minute song (3 minute would be around 80 measures). It took a while but I choosed rock, since I am very familiar with this type of music.

I started to experiment what kind of song I could make, trying out different samples and seeing what worked, like this for example:

```
from earsketch import *

init()
setTempo(120)

for measure in range(1,9):
  fitMedia(OS_OPENHAT01,1, measure + 0.5, measure + 1)
  fitMedia(OS_CLOSEDHAT01,2, measure + 0.9, measure + 1)
  
  finish()
  ```
A slow, simple hi-hat beat to start things off. By now, I was finally starting to understand how useful the `for measure in range` command was. Afterwards, I started experimenting some more and made this:

```
init()
setTempo(120)

fitMedia(Y01_HI_HATS_1,1,1,9)
fitMedia(Y01_KICK_1,2,1,9)
fitMedia(Y01_SNARE_1,3,1,9)

setEffect(1, WAH, WAH_POSITION, 0.3)

finish()
```
This time, I was simply figuring out what other SFX I could make. I tried out distortions, reverbs, pitch changes, etc. Finally, the most recent drum pattern I tried making was this:

```
from earsketch import *

init()
setTempo(82)

kick= Y01_KICK_1
beat1= "000+-+000+-+"

for measure in range(1,9):
 makeBeat(kick, 1, measure, beat1)

fitMedia(YG_FUNK_HIHAT_1,2,5,9)

finish()

```
Overall, this week was me experimenting some drum patterns I could use for the song in question. I still haven't decided a specific one yet, but once I do, I plan on figuring out bass samples I could use next.

### Conclusion
---
When experimenting with a new coding program, try to make something after a while. Even if it's just a portion of the bigger project, it's good to constanly plan what your next idea will be. Don't be afriad of trial and error; you're gonna make mistakes along the way, but use that as fuel to learn for the future.