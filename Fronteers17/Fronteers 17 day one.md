#Fronteers17 day one 5 October 2017

## Don't panic – [Niels Leenheer](https://twitter.com/html5test)

Different brouwsers & different rendering engines doesn't force you to support them all.
We can use progressive enhancement, but when is something part of the core experience?

(interactive) Animation header? could easily fallback to a static image.
Animation in an icon (svg) also, you don't **need** the animation.

Don't forget who you are building for! Know your users and build for them!
_delight your users_

[Slides](https://speakerdeck.com/nielsleenheer/dont-panic-at-fronteers-conference-2017)

## Imposter Syndrom & individual competence – [Jessica Rose](https://twitter.com/jesslynnrose)

## A modern Front-end Workflow – [Umar Hansa](https://twitter.com/umaar)
ModernDevTools.com

- `Cmd+shift+p` type `screenshot` for a full page screenshot
- Contrast ratio in the colorpicker
  - contrast icon gives more info about the contrast
-  Is the text over an image the new version has a colorpicker for the background-color
- Verbose logging for best practice warnings
- Audit tab to audit structure

#### Quantify damage by third party scripts
- Performance panel & throttle cpu
- start recording
- Summary pane gives rough amount of time for loading & scripts (large amount of scripting)
- Go network & block request domain for suspected performance issue
- Scripting time is dropped quite large
- You can also switch to previous recording


- Canary `cmd+ shitft+P` -> enable experiments
- hit shift 6x for more options

## Caches All the way down – [Yoav Weiss](https://twitter.com/yoavweiss)
_Cache is important_
- Immutable content
  - version them
  - max age 3xxxxxxxxxx or immutable
  - Change version or hash on new version
- Always revalidate with max age of e.g. 5


## Debugging Accessibility — [Alice Boxhall](https://twitter.com/sundress)

#### courses/info:
- http://bit.ly/web-a11y
- http://bit.ly/a11y-fundamentals

- Disability is an **interaction**

**Make your site**
- Perceivable
- Operable
- Understandable
- Robust

Look to the 'default' interaction en don't change anything in that.
For example an dropdown, crating an visual alternative make sure the usage stays the same.
Not just with the mouse but also keyboard navigation.

On icon-based navigation items it's important to use screenreader items.

#### Ally check explore DOM tree
[bit.ly/devtools-a11y-pane](https://bit.ly/devtools-a11y-pane)
Chrome flags devtools enable accessibility

`list-style: none;` has accessibility implications in some browsers.

**“The less an interface requires of its users, the more accessible it is.”**

**ARIA is like a polyfill, only use it when you need it.**

## 1Up your writing with plain language — Ashley Bischoff
W3C accessibility guidelines has sentences of more then 40 words.
The complexer the subject the shorter the sentences should be.

## Honey, I Shrunk the Scripts! _Exploring the javascript microworld_ — [István "Flaki" Szmozsánszky](https://twitter.com/slsoftworks)

NodeJS started the JS + Hardware movement.
JerryScript is a very small JS engine for a microcontroller.

## Perfectly portable 2.0 – [Jennifer Geacone-Cruz](https://twitter.com/anomiseditrix)
[@Lingvist](https://twitter.com/Lingvist)
[@Feeldco](https://twitter.com/Feeldco)
