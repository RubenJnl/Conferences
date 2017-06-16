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

[Slides](https://rachelandrew.co.uk/speaking/events/css-day-nl-2017)