#Fronteers16 day one

## Progressive Enhancement and CSS | [Ire Aderinokun](https://twitter.com/ireaderinokun)
[Bitsofco.de](http://bitsofco.de)

Points for progressive enhancement
- Content accessible for all browsers
- Semantic markup
- Enhanced layout can be provided by css
- Enhanced behaviour with js, !not primary
- Respect web browser preferences

Use JS?
- Only as enhancement, do not braik main functionality without JS
- Feature detection
	- Polyfill, just like we do only load if necessary 

Markup is core

_Confirmation of our use:_ 
- *Media queries with min-width for enhancement*
- No magic nubers! :) 
- Flexbox FTW as progressive enhancement, overrules all others like display table.

New features detect with ```@supports``` or just no support
``` 
@supports not ( display: flex; ) {
  .u-flexy {
    display: table;
  }
}
```

## Hacking the visual norm | [Nadieh Bremer](https://twitter.com/NadiehBremer)
[VisualCinnamon.com](http://visualcinnamon.com)

Visualisation tool [d3.js](http://d3js.org)

Mandatory rainbow phase just for fun when starting data visualisation :')
Data sketch|es

Copy, Transform, Combine -> Everything is a remix

[Slides](https://nbremer.github.io/hackingthevisualnorm/)


## 	How You Do What You Do Is Who You Are | [Scott Olson](https://twitter.com/gscottolson)
Levering React JS to improve user experience.

### Preloading images
Default preload image as source, on load you can fade the image. Of broken you can set a custom image.
```
div - width: 33.3%, position: relative
IMG spacer - width: auto; height: auto;
```
```
<svg width=4
height=3
viewbox 0 0 4 3 />
```

With a preloader you can order the loading of images.
example: You can just request the first 6 images instead of setting the source for all xx images on the page.
 
Dynamic input sizes
Default
- explicit size
- explicit percentage 

Set opacity for the input to 0 and fill the span with the input, the span has the right behaviour for autosizing based on content.

Using placholder text inside input as we know isn't a great thing when you're hiding labels.
On focus/value!="" the placeholder will disappear.
Animation like we do on DLLDealerlease/LEASIT is great for the user experience. The label appears above the input when focussed or filled inputs.


## Offline, progressive, and multithreaded: a peek at the webapps of the future | [Nolan Lawson](https://twitter.com/nolanlawson)
[Slides](https://nolanlawson.github.io/fronteers-2016/#/)

HTML5 was a response to Flash

Progressive Web Apps are a response to native mobile apps.

Dynamic data storage in the browser

LocalStorage is depricated, only strings and synchronous. IndexedDB is Async and transaction based.
"There are three pilars for the web; HTML, CSS and JS. You can't yank one out and expect everything to work".
 Maybe not everything but what about accessibility? 
 
In the end: Build a better experience for the user!


## Multi-user WebVR or: Wait, Who Are These People? | [Martin Splitt](https://twitter.com/g33konaut)

"Vomiting because of VR motion sickness: *a bucket full of fun!*"

### Devices
- Gear VR
- Cardboard
- Occulus
- Steam VR 

Buisinesscase for VR?
- education
- marketing
- construction/architecture
- healthcare
- design/art

### WebRTC 
- Low latency direct communications between devices.
- signalling through server first

### WebGL
- rendering a lot of pixels on the screen for 3D

### WebVR
- Get a list of displays and render canvas on the displays

#### Framedata for VR contains
- Pose
  - Orientation
  - Position
- Projection matrix for each eye _don't worry what it is, just use it_

And that's the WebVR API

### Where are we with VR?
- Current draft 1.1
- <3 from Mozilla, Google, MS & Samsung
- Experimental browser builds
  - No VR there's just a single picture
- Gamepad API extension
- No DOM just yet

[Slides](https://docs.google.com/presentation/d/1h1JeRFoxL_Vp4hFQrsqvGe-tM-02PPMG5p9tBwpW-bQ/edit#slide=id.p) [ShortUrl](http://bit.ly/fronteers-webvr)
^^ contains links to great VR resources

## Big Data, Big Impact | Lodewijk Nauta


## Scaling Front End Development | [Monika Piotrowicz](https://twitter.com/monsika)

FED isn't living in a vacuum, always working together with other disciplines.

### WTFED?
Previous:
- HTML, CSS, JS
Now:
- Node/WebPack/Sass/Gulp/PostCSS/CoffeeScript/a11y/SVG/Bower etc...

What happens when the FED role doesn't exist?
Design --------- | -------- AppDev
| HTML, CSS, JS -> who's responsibility?
- It's the User Interface, THE fine line between the back-end and the user.
- inconsistent or even buggy
- spaghetti code
- hard to maintain & iterate
- not accessible/performant/responsive

Owners of a spectrum, you can fall between Design & FED or between FED and Back-end

### Building a craft
1. Language styleguides
  - shared coding standards
  - consistency is key
  - helps team members reach each other's code
  - helps rethinking how you code

2. Code reviews
  - support & grow your guide
  - standards to make things easier
    - if hard to enforce, it might not be useful
  - shared definition of quality
  - builds a culture of *feedback and knowledge sharing*

3. 

### What to include?
- A common stack(s)
- responsive guidelines - easy defaults for breakpoints, grids, testing
- performance standards & language tooling
- accessibility best practices

### UI library
- core application patterns, built in a reusable way
- solve for our use cases

### Why bother creating UI patterns?
- Solve problems once
- more people can contribute
- more time on most impactful features

## 	Surveying the Landscape | [Peter Gasston](https://twitter.com/stopsatgreen)
Universal links for App's on iOS
Medium is pushy about using the app
e.g. NYTimes - App is clean and the website is cluttered

Advertisement represent 9% on the page 54% load & 55% bandwidth.

[Google AMP](https://www.ampproject.org/)



## Other notes
- [Pim Derks](https://gist.github.com/PimDerks/d2b339d567ab0759fc2e648dcd3c4c19)
- [Nienke Dekker](https://github.com/nienkedekker/fronteers-2016)
