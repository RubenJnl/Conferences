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


## Building Responsive CSS Components | [Zell Liew](https://twitter.com/zellwk)
Make components scalable, but how?

Main typo in REM/VW and the rest in EM. _No need for our baseline?, at least not for font-size. We still need margins to be relative to that._

Limit the number of font-sizes
Repeat the baseline, just like we already do.
- Lineheight for e.g. 24px
- Heading = 48px
- Extra spacing is + 24px or 1/2 or 2x that

Size in EM if the property is relative to font-size.

Everything else scale in REM

Extract the repeating styles to mixin's if needed.
- Determine component area maps.
- Determine breakpoints and changes in styles
- Determine units for CSS properties
- Handle complex variations with mixins (or element queries in the future)
- But especially: Don't over engineer!

### Other notes
[Bram Willemse](https://workflowy.com/s/Ji590S8RDz)


## CSP STS PKP SRI ETC OMG WTF BBQ (Modern websecurity standards) | [Scott Helme](https://twitter.com/Scott_Helme)
HTTP/2 Security features: only over https
- Geolocation 
- getUserMedia
- AppCache
- Brotli Compression (better then Gzip)
- SEO Boost 


## 	Functional Animation | [Sarah Drasner](https://twitter.com/sarah_edo)

Invisible VS Immersive animation
### Invisible animation
Connecting states with smoothstate.js?
Morphing state x to state y to state z with svg animations.

Animate from modal anchor to modal window.
Keep de user busy, like an loading indicator. With a custom loader waiting time is even longer.

Opacity en Transforms trigger the least amount of repaint.

### Immersive

DOM/VirtualDOM
Pros
- Great for UI/UX animation
- Great for SVG (resolution independent) 
- Easier to debug
Cons
- tanks with a lot of objcts
- Care about the way you animate

CANVAS
Pros
- Dance, pixels dance
- great for impressive 3D
- Movement of tons of objects
Cons
- Harder to mak accessible
- not resolution independent _out of the box_
_ breaks to nothing

### SVG
- Crisp on any display
- Less HTTP requests
- Easily scalable
- Small file size (performance)
- easy to animate
- easy to make accessible


## 	World-Wide Web, not Wealthy Western Web | [Bruce Lawson](https://twitter.com/brucel)





## Other notes
[Pim Derks](https://gist.github.com/PimDerks/fc2b3c30e8b7a985a496512eda705079)
[Ian van der Wiel](https://github.com/iainvdw/fronteers-2016-notes)