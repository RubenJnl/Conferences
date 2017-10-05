#Fronteers17 day one 5 October 2017

## Don't panic – [Niels Leenheer](https://twitter.com/html5test)

Different brouwsers & different rendering engines doesn't force you to support them all.
We can use progressive enhancement, but when is something part of the core experience?

(interactive) Animation header? could easily fallback to a static image.
Animation in an icon (svg) also, you don't **need** the animation.

Don't forget who you are building for! Know your users and build for them!
_delight your users_

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

## Caches All the way down – Yoav Weiss
_Cache is important_
- Immutable content
  - version them
  - max age 3xxxxxxxxxx or immutable
  - Change version or hash on new version
- Always revalidate with max age of e.g. 5


##
