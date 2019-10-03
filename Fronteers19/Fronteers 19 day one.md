#Fronteers19 day one 3 October 2019

## [Charlie Owen](https://twitter.com/sonniesedge) – All Constraints are Beautiful
Constraints are everywhere. Not just people but also technology.
For example low battery, screen size/type.
Even small things can be a disability, think about colourblindness, prescription glasses or even a temporarily disability like a broken bone.
> We don't have disabled users

Over 50% of all users have at best a mid-range device. Make sure it's running smooth and fast.
> Progressive enhancement is sexy as fuck
_^^ you know wat this means_ (make it work on low-end devices)

Client side rendering break easily. HTML & CSS is robust!

> A Simple Site Is A Resilient Site
Does it need to be resilient?
If it's not resilient will ...
... it endager the life of a user?
... it cost a user money?
... they suffer legally?
... their job be impacted?
... they time-penalised?

*Users before Engineering*

> Fuck facebook and their friends!
We know the constraints and we can do better!

## [Chen Hui Jing](https://twitter.com/hj_chen) – A deep dive into images on the web

[Slides](https://www.chenhuijing.com/slides/71-fronteers-2019/)

––––––

## [Christophe Porteneuve](https://twitter.com/porteneuve) – Fun & Games with ES Proxies

`[object].hasOwnProperty(target)`
`has(target, prop)`
Get boolean of target inside object.

`ownKeys(target)`

[Immer](https://immerjs.github.io/immer/docs/introduction)

[Slides shortURL](bit.ly/fronteers-es-proxies)
[Slides](https://deliciousinsights.github.io/fronteers-es-proxies/#/mainTitle)


## [Eva Lettner](https://twitter.com/eva_trostlos) – Paint the web - Drawing with CSS
> Code is magic ✨

======

## [Jad Joubran](https://twitter.com/JoubranJad) – Secrets of native-like PWAs
From the users perspective the app is not about the technology.
It's about the experience. Is it smooth from start to end?
If done right, even developers can't tell the difference.

###Pillars of native-like PWA's:
User Interface, User Experience (and Performance) & Reliability

It's successful if it exceeds the user Experience.
For a shell limit to 20kb or less inline code

###TAB BAR benefits
It simplifies the interface/navigation

use module for app, and legacy with a nomodule js
```
<script type=module src=app.js></script>
<script nomodule src=app-legacy.js</script>
```
Also split different types of js like:
home,
vendor,
settings,
help,
payment

```
/// show loader when loading settings
/// after 3s switch loading message to "still loading".
/// retry for critical modules witch .catch
import('settings.')
.then(module => {
  module.init();
});
```

`requestIdleCallback(()=>{})`
Defer non-critical work, might want to test before/after using.

Offline
always use networkTimeoutSeconds, if connected to router and that's not on internet it fails without max timeout.

Apply updates like chrome/spotify with a small colorchange or dot. It's all in the details.

[Slides](jadjoubran.io/fronteers19)

## [Rachel Andrew](https://twitter.com/rachelandrew) – Who Designed This? Where Web Platform features come from, and how to get involved
### GO get involved with feedback, testing etc...
[Slides](noti.st/rachelandrew)

## [Stephen Cook](https://twitter.com/StephenCookDev) – 100% CSS Mario Kart


[Slides](https://stephencook.dev/slides/mario-kart-css-talk/)

––––––

## [Paul Lewis](https://twitter.com/aerotwist) - Custom Web Shadow Elements, or whatever...

## [Jeremy Keith](https://twitter.com/adactio) & [Remy Sharp](https://twitter.com/rem) – How We Built the World Wide Web in Five Days
