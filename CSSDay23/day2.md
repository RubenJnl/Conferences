#CSS Day – day 2

# Container Queries – Miriam
normal flow is how the web supposed to be before some sh*thead decided to add a 1024px width

contain layout also contains z axis
just set container-type size or inline-size

name containers queries you can skip the nearest containers to like 2-3 levels above
"turle containers" elements that carry their own container
you can use :host

# Modern css development – Umar
create code snippets from new features & other predefined settings *photo
bloop.ai for q&a & suggestions.
MacWhisper?

vscode sticky scroll! keeps selector on top
expand-region, expands selection to selector
live-preview plugin
 jumpy / acejump

cmd shft p - experiments - style sync
sources - filesystem sync from devtools to project

devtools snippets performance
accessibility devtool snippets


# building components – Stephanie

css nestng cant use an element should be a symbol
wrap :has in :where reduces specificity!
https://noti.st/st3ph/ea40FC/modern-css-for-dynamic-component-based-architecture#syPitwA


//lunch 

# Creative Coding – Jhey
awesome css (scroll) animation demos


# Styling web components – Cassondra
webcomponents - use libraries like lit for prd
window.customElement.define("Card", Card) // can only be defined once!
i
use default semantics instead of custom components;
class WordCount extends HTMLParagraphElement {}
.define("wc", Wc, "p")

# Scroll driven animations & View transitions – Bramus
view transition creates snapshot of current and new state, then fades to new.
simiple example; https://codepen.io/bramus/penI/WNYNKmg?editors=0110 
Interupted transitions skip to the end

https://scroll-driven-animations.style/
scroll driven is smoother then scroll triggered


# Structuring & Restructuring – Manuel
custom properties easy; color vars
day 92 for color re-use: https://www.matuzo.at/blog/2023/100daysof-day92/
BEM to BAPI (block & api)?
100vh = large, use of dvh (denamic viewport) blog day 38
scrollbar-gutter: stable; day 20 & 25

maysonry day 71 & 72

overflow: clip; on an open dialog prevents page scroll

