#Fronteers16 day two

## Adapting to Input - [Jason Grigsby](https://twitter.com/grigs)

It's not just keyboard and mouse anymore
Touch, Multi-touch, Camera, GPS, Bluetooth (LE), compass, accelerometer, etc..
Also think about gestures & voice control.
 
How are we going to use gestures or predictive touch?

### Why should we detect touch if we don't detect mouses and keyboards?
- Mouses/keyboards can be added/removed easily.
- You can use touch the first moment and a mouse the next.

Fitts's Law
The time to aquire a target is a function of the distance to and size of the target.

Design for interaction, not input.
You're designing for user need, not a specific form factor or input.

Using a remote can be the same as using arrow keys. (you can't detect a remote).

### Abstract baseline input
Like mobile/tablet/desktop (small/medium/large)
Focus on point/select instead of tap/click

jquery pointer events polyfill ([PEP](https://github.com/jquey/pep))

Safari can fill CreditCard info from the camera.

### Add apple pencil to the devicelab
"No device testlab inhouse, just go to the Apple store" 


[Slides](https://speakerdeck.com/grigs/adapting-to-input)
[Notes from Bram Willemse](https://workflowy.com/s/QRnBToXi7o)


## Cheat Sheet to a Lean Website - [Barbara Bermes](https://twitter.com/bbinto)
People don't like to wait.
Abandoning websites because of slow loading is high.
Especially after like 10 seconds "Forget it I'll leave"

### Treat speed as a feature
This should not be a "Nice to have" but a "Must have"
Optimize from a user's prerspective, look at the target group.

What about energy saving?

CRP (Critical Rendering Path) 
- Clean HTML √
- Cleanup DOM bij removing unused elements
- encode/compress images √
- avoid custom webfonts
- Use Gzip
- Reduse HTTP requests
- Image sprites _really? it isn't 2010 anymore_ Think about the mobile web & retina, maybe svg sprites is an alternative. 
- Use CDN's
- Offline storage
- Prevent redirects (DNS lookup)

What we're already doing
- Async/defer js loading
- scripts at bottom of the page to prevent render blocking
- Concatinate JS

### monitorring loadtime is important
Like when ads/tracking is added and loadtime shoots through the roof.



## Other notes
[Pim Derks](https://gist.github.com/PimDerks/fc2b3c30e8b7a985a496512eda705079)