# Entry 7: Continuing the Project (Part 2)
---
Continuing with what I left off with, I've been experimenting more with how I'd want this song to sound. I haven't thought of a definite plan, but what I've made so far is interesting.

Firstly, I changed up the intro a bit, by switching around the tracks measure. It's still a work in progress, but I hope to come up with something that can sound satisfying

```
for measure in range(1,17):
    makeBeat(track, 8, measure, beat1)
    
fitMedia(Y11_KICK_1,3,9,17)
setEffect(3, VOLUME, GAIN, -4.0)
fitMedia(RD_ROCK_POPLEADSTRUM_GUITAR_9,4,13,26)
setEffect(4, VOLUME, GAIN, -8.0)
```

Also, I started working on the bridge of this song:

```
fitMedia(RD_ROCK_POPELECTRICBASS_7,9,26,34)
fitMedia(RD_ROCK_POPLEADSTRUM_GUITAR_10,10,26,34)
setEffect(10, VOLUME, GAIN, -8.0)
setEffect(9, VOLUME, GAIN, 4.0)
```

This week has shown me that part of the process of making music  is experimenting. Experimenting can lead to a lot of interesting outcomes that you never would have thought of in the first place. But, that's just from my personal experience, since I think making music varies for everyone.

# Conclusion
---
Sometimes, experimenting freely can work better than planning everything out. Sandbox a lot. There's a lot you can learn from testing code and seeing what works and what doesn't. 