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

