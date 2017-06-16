#CSS Day two

##CSS Reset | Bert Bos & [Håkon Wium Lie](http://twitter.com/wiumlie)
Collapsing element
Border radius is just opsmuck

## CSS Grid | [Rachel Andrew](http://twitter.com/rachelandrew)

March 2017 Grid layout shipped in all mayor browsers (Except Edge, only prefix for now)
Worldwide almost 64% support, with prefix Edge like 75%

"The more I know about CSS, the more I realise I don't know" – Rachel Andrew

Outer and inner display type, how does the box behave in realtionshop to parent and how does the item respond to changes.

Whe applying a grid, all items (block, inline, etc.) change to grid items and take the specified layout in the grid.
Display table as fallback for older browsers.

Subgrid solves the problem of vertical aligning items inside grid items when it's implemented.
Display contents fixes this partially, but be aware: all box styling will be removed.
 
Grid is writing mode aware, it changes position when you are 'rtl'.

useful links:
[grid by example](https://gridbyexample.com/learn/)
For more see [Rachel's twitter and search for #CSSDay](http://twitter.com/rachelandrew)

[Slides](https://rachelandrew.co.uk/speaking/events/css-day-nl-2017)


## Designing Grids | [Mark Boulton](https://twitter.com/markboulton)

"When technology matures creativity comes around the corner"

Grids provide order, connectedness and reinforce hierarchy.
The point of grids is to connect space.

You can't just design a grid and you're done.
You can do everything you want, even uneven columns. Bot rewrite it the moment it doesn't look good anymore.

"Change the grid to suit the content"

"Baseline grids where designed for very large multiple columns like newspapers, so actually don't bother using them" 

Odd numbers prevail, because they simply look better. 
You can also use an even grid and just don't put content in one column

Hanging line is a top line you hang your content on. Great for the reader, give them a break. Show them this section is done.

When you use a line between grid colums/rows, make sure your gutters are like 31 or 21px.

"Experiment with grids, especially designers"
“Adapt what is useful, reject what is useless, and add what is specifically your own.” – Bruce Lee


## Writing Modes | [Jen Simmons](https://twitter.com/jensimons)

New proposal on display: outside inside;
Draft for run-in looks great, you can place the dt in the front of the content of the following dd in a definititon list.

Direction should NOT be used in css but in your html tag `dir="ltr"`
When using float you also need to change left to right and the other way around. Here flexbox/grids come along, but we already know that.
bdo/bdi (block and inline direction change for a specific section)

Exceptions from default ltr/rtl are:
Block direction is ltr and inline direction is top -> bottom for example Mongolian
Chinese, Japanese, Korean (HAN-based systems) they usually use block direction rtl and inline direction top -> bottom

Writing mode has 3 options:
- horizontal-tb 
- vertical-lr (not used regularly)
- vertical-rl

Example for not using up the vertical space:
```writing-mode:vertical-rl;
text-align: right;
text-orientation: sideways;
transform: rotate(180deg);
```

text orientation is not well implemented everywhere but it's good enough.

Bungee, fonts for vertical and multicolor!

