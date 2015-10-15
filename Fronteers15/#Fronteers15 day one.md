#Fronteers15 day one


## 1. Delivering Responsibly - Scott Jehl
- Fluid screensizes, no more specific sizes.
- 2 and 3g mobile connections are still more a standard then 4g, make sure to take that in account.
- Also take performance/battery use in concern.
- More mainstream ways to block JS, make sure it works without.
- APP: Purify (contentblocker)
- Don’t forget to use img srcset for images ;)
- Inline css above "the fold” to improve rendering, use only critical css here.
- Critical css: github filamentgroup grunt-criticalcss
- High priority JS?: Polyfills, Feature test, but ideally: none
- LoadCSS -> async load css
- ?Add class to change font to webfont when the font is loaded? -> Future css: font-display: swap;


## 2. Digital Governance - Lisa Welchman
- know who's responsible for each descision.
- It doesn't take of if you don't have standards, make sure you have standards


## 3. Lightning Fast Sass - Chris Eppstein
- npm i node-sass
- eyeglass is npm support for sass, you can use js for sass. //eyeglass.rocks
- Eyeglass spriting, use separate images and eyeglass will render the sprite


## 4. Walking the Tightrope Between Mediocrity and Bankruptcy - Primate
- embrace progress, create for content, be honest


## 5. jsmpeg: Why a JavaScript Video Decoder Actually Makes Sense - Dominic Szablewski
-


## 6. Front-end Style Guides - Anna Debenham
- Styleguides will help you after finishing a project. Especially when someone else is working on the project. With a styleguide you'll give them de design descisions you've made. Especially for new people/starters who don't know all the best practices.
- Good guidelines tell you what to do, great ones will also give you a reason. And excellent guidelines will give you further reading on those reasons.
- Make it public: forces you to maintain it. Also helps with requitment. Lets others comment on your styles.

## 7. What is the Business Case for Accessibility? - Alice Bartlett
- impairments: visual, motor, hearing, (focussing)
- Building fron scratch, why wouldn't you make it accessible? You just need to know the basics. (tab index, skip links with correct id's etc..)
- 4 Levels of accessibility:
	- Don't screw op the HTML: properly structured html gets you 90% of the way!
	- Check with tools: wave (web accessibility evaluation tool) or Tenon.io
	- Test wish assistive tech: use a screenreader! JAWS,NVDA,VoiceOver (Mac), ZoomText, Window-eyes
	- Ask an expert!

- Chrome accessibility tab! chrome://flags/ enable accessibility inspection!
- aria hidden to hr's for example


## 8. Modern Progressive Enhancement - Jake Archibald
- Don't block lines with big fat scripts! (test with network throttling on)
- Make your markup, don't use JS primary to show the first content. Even in an app!
- Unblock your scripts async or defer attribute (defer not for IE9!)
- Don't block painting with webfont loading! new font-display:optional :) for now use filamentgroup async css?
- Async load all css and inline first styles
- HTTP/2 doesn't have a large overhead like HTTP on async loading small files.
- 