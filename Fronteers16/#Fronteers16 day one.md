#Fronteers16 day one

## Progressive Enhancement and CSS | Ire Aderinokun
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

## Hacking the visual norm | Nadieh Bremer
[VisualCinnamon.com](http://visualcinnamon.com)

Visualisation tool [d3.js](http://d3js.org)

Mandatory rainbow phase just for fun when starting data visualisation :')
Data sketch|es

Copy, Transform, Combine -> Everything is a remix

## 	How You Do What You Do Is Who You Are | Scott Olson
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

## Offline, progressive, and multithreaded: a peek at the webapps of the future | Nolan Lawson
[Slides](https://nolanlawson.github.io/fronteers-2016/#/)

HTML5 was a response to Flash

Progressive Web Apps are a response to native mobile apps.

Dynamic data storage in the browser

LocalStorage is depricated, only strings and synchronous. IndexedDB is Async and transaction based.
"There are three pilars for the web; HTML, CSS and JS. You can't yank one out and expect everything to work".
 Maybe not evertything but what about accessibility? 
 
 


