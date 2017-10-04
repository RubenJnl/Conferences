# Fronteers17 workshop 4 October 2017

[slides](gool.gl/TRwzZF)

## Classic animation theory
_The 12 Classic principles_

- Book: Disney animation — the illusions of life —
- [the12principles](https://the12principles.tumblr.com)
- Book: Richard Williams — The animator's survival kit

## [Classic principles worth stealing](https://www.slideshare.net/secret/1yK01w1F4bNpNz)
### Timing & Spacing
- Timing = duration
- Spacing = easing

`cubic-bezier` is motion's best friend.
But... magic numbers :fearful:
Sources:
- [cubic-bezier](http://cubic-bezier.com/)
- [framer-js playground](https://stakes.github.io/framerplayground/)

### Mass & Direction

### Follow Through / Overlapping action
_Not everything stops at once_
- Different parts of the "body" move at different times
- Overlapping action could be important
  - don't wait til the first is done `e.g. score modal, start score before moving in modal`

### Anticipation
- a little hesitation before main movement `e.g. little move back`
- Preparing for the main move
- _Gives the feeling the object is moving itself_
- more info by Val Head's [motionandmeaning podcast](http://motionandmeaning.io/)

### Arcs
- Organic movements typically don't follow straight lines

### Secondary action
- Reinforces the main action (supports)
- medium applause or twitter heart are great examples.

### Exaggeration
- Make it bigger then it is to draw attention
- The "truth" but more extreme

### Appeal
- The charisma of the action
- Makes you like or particularly appreciate an animation

### Squash & Stretch
- Gives a sense of weight and flexibility
- Object tend to change on movement
- It's important to keep the volume of the object

### Staging
- Directing the audience's attention to the most important thing in a scene
- Focus on animation before loading content
- Rotate in the direction a list is opening in

## Beyond the twelve
### Choreography
- Making things work together, follow-up, secondary action, anticipation
- Similar objects move in similar ways `e.g. thumbnails moving from same direction, not `
- Entrance informs exit; enters from bottom, moves away to bottom.
- Action confirm to top cancel back to bottom
- Match velocity like top speed not the time of the duration, whether it's longer or not.

### Consistent & Cohesive
- Consistent: Same followthrough/same bezier for easing
- Cohesive: Same upward direction

### Continuity
- Visual Continuity
- Reuse elements between views
- Planning entrance & Exit movements v.s. fading to black each time

# CSS Transitions
Three things in CSS
- [Transforms](https://developer.mozilla.org/en-US/docs/Web/CSS/transform) _Does not make things move by itself_
- Transitions
- Animation

## [CSS Transforms](http://slides.com/vlh/web-in-motion-fronteers?token=zhiyqQq1#/5/3)
- Transform order follows order of properties
- [Matrix](http://meyerweb.com/eric/tools/matrix/) from transform properties
```
scale(2) translate(50px, 100px) skew(30deg) rotate(90deg)
// equals to
matrix(1.1547, 2, -2, 0, 100, 200)```
- A lower perspective number makes the `rotateX` more drastic
- you can use `perspective` on the parent
```
.parent {
  perspective: 100px;
  transform-style: preserve-3d; // optional
}
.child {
  transform: rotateX(45deg)
}```
- BounceJS helps you create matrix transforms

## CSS Transitions
- From point A to point B
- You need a duration

## Keyframes
-  `animation-fill-mode: both;` keeps the start & endstate

## CSS Varibles
- Can be set with JS. you can set like `--mouse-x` & `--mouse-y` and use it directly with CSS
-

# SVG Workflow & Animation
- SVG optimized paths are terrible for animation.
- Use different groups/elements
- Inline SVG For animations

https://jakearchibald.github.io/svgomg/
https://petercollingridge.appspot.com/svg-editor/

### export SVG from Illustrator
- Internal CSS gives a block of CSS
- Inline styles === inline `style`
- Presentation attributes like `fill` in the paths
- Font SVG gives you live text even with webfonts
- Convert to outlines in export only
- Object ID's are set to the layer names

### Optimize SVG
- Weird exported icons could happen by not enough decimal places, the smaller the icon the more decimal places
- With optimizing don't optimize shape to paths. A path can't change radius like a circle

### Animating SVG with CSS
- Layers are stacked upon eachother, last item has highest z-index
- If the viewbox is to small you can use `overflow:visible;`

### Animating SVG with JS
- Different browsers use different transform origins libraries can fix this for you.
- [drawSVG](https://greensock.com/drawSVG) More control over line drawing like the [stroke animation](https://codepen.io/valhead/pen/oXNaBW)
- [morphSVG](https://greensock.com/morphSVG) like morphing circle into elephant

[Easing visualiser](https://greensock.com/ease-visualizer)

### Performance
**Efficient:**
- size - transform: scale()
- position - transform:  translate()
- rotation - transform: rotate()
- opacity

What effect's what? check [CSSTriggers](https://csstriggers.com/)
