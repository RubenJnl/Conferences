#CSS Day one Browser API Special

## Animations | Rachel Nabors

Timing & Movement
When & Where
Stateless animation
- Frame rate independent, always animates in given time
- Directiin Agnostic (go forward, backwards, repeat, etc.)
- Seek-able
- 

API benefits:
- onfinish 
- oncancel 
- ready
- playState
- playbackRate
- ready
- currentTime (time & location)
- finished

https://codepen.io/rachelnabors/pen/35936ab4c3be0a82fc82e460601268da

It is possible to speed up animations from your browser with the playBackRate.

api desc: https://developer.mozilla.org/nl/docs/Web/API/Animation
more specific on animation then caniuse: https://developer.microsoft.com/en-us/microsoft-edge/platform/status/
[Web animation api polyfill](https://github.com/web-animations/web-animations-js)
[Slides](https://www.slideshare.net/CrowChick/alice-in-web-animations-api-land)


## Form validation | PPK

[Info & demo](https://www.quirksmode.org/forms/)

trick; input:invalid:not(:focus)
Block label
```
<label>
  Your name
  <input type="text" required />
  <span>Your name is required</span>
</label>
```

[Slides](https://quirksmode.org/presentations/Spring2017/formvalidation_CSSDay.pdf)

### Notes:
https://make.wordpress.org/accessibility/2017/01/16/testing-form-functionality-with-different-assistive-technology/


## Houdini & Polyfilling CSS | Philip Walton

CSS polyfill writes code that the browser does understand

[Slides](https://github.com/philipwalton/talks/tree/master/2017-06-15)


## Web Audio | [Ruth John](http://twitter.com/Rumyra)

[Blokdust | webAPI demo](https://blokdust.com/)

Load sounds, 3 ways:
get from dom
get a stream
Fetch to buffer

These three output a source
source connect and then start.

Firefox devtools has an audio tab

Howler.js, also supports sound spriting.

[Slides](https://github.com/Rumyra/Talk-Web-Audio)


## WebVR | Ada Rose Edwards

Watch out for the samsung internet browser, it's the 3th most used browser in Europe. So test!

[Simple VR Demo](http://o.ada.is/simple-vr)
[VR Demo 1](https://o.ada.is/vrdemo1)
[VR Hackathon](https://medium.com/samsung-internet-dev/virtual-hackathon-lets-make-vr-together-53f629552764)

[Slides](http://o.ada.is/css-day)


AFrame for creating 3d objects
With webvr you can bring audience together.


## Weird APIs | [Mike Taylor](https://twitter.com/miketaylr)

[Boolean trap](https://ariya.io/2011/08/hall-of-api-shame-boolean-trap)

[Slides](https://miketaylr.com/pres/browser-api-day/)


## Progressive web Apps | [Patrick Kettner](http://twitter.com/PatrickKettner)

[Hushlittlebaby -> instead of 45MB video](https://hushlittleba.by/)

[Browser storage abuser](https://demo.agektmr.com/storage/)
Check how big your cache can get.

node js: manifestatioon -> create web manifest
[webmanifest generatoo online](http://webmanife.st/)
[validator](http://webmanife.st/validator)
[spec](http://webmanife.st/spec)

Web payment request for native payment instead of a bulky checkout. 
[More info at google](https://developers.google.com/web/fundamentals/discovery-and-monetization/payment-request/) 




# Other links; 
[Flexbox bugs](https://github.com/philipwalton/flexbugs)