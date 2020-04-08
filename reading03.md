[README.MD](README.md)  

**Flexbox**  

- The Flexible Box Module, usually referred to as flexbox, was designed as a one-dimensional layout model, and as a method that could offer space distribution between items in an interface and powerful alignment capabilities.  
- When working with flexbox you need to think in terms of two axes — the main axis and the cross axis. The main axis is defined by the flex-direction property, and the cross axis runs perpendicular to it. Everything we do with flexbox refers back to these axes, so it is worth understanding how they work from the outset.  

_key words/ commands and def_  

-  __*Display*__  defines a flex container; inline or block depending on the given value. It enables a flex context for all its direct children.  

- __*flex direction*__  Establishes the main axis defining the direction flex items are placed in the flex container.

- row (default): left to right in ltr; right to left in rtl  
- row-reverse: right to left in ltr; left to right in rtl  
- column: same as row but top to bottom  
- column-reverse: same as row-reverse but bottom to top  
- __*flex-wrap*__  flex items will all try to fit onto one line. You can change that and allow the items to wrap as needed with this property.  
- __*nowrap*__  (default): all flex items will be on one line
- __*wrap*__: flex items will wrap onto multiple lines, from top to bottom.  
- __*wrap-reverse*__  : flex items will wrap onto multiple lines from bottom to top.  
- __*flex-direction and Flex-wrap*__ together define the flex containers main intersecting axes.  

__*justify-content*__  defines the alignment along the main axis. It helps distribute extra free space leftover when either all the flex items on a line are inflexible, or are flexible but have reached their maximum size. It also exerts some control over the alignment of items when they overflow the line.  

[https://css-tricks.com/snippets/css/a-guide-to-flexbox/](CSS-tricks)  (definition credit)  

- __*flex-start*__ (default): items are packed toward the start of the flex-direction.  
- __*flex-end*__  : items are packed toward the end of the flex-direction.  
- __*start*__ : items are packed toward the start of the writing-mode direction.  
- __*end*__ : items are packed toward the end of the writing-mode direction.  
- __*left*__ : items are packed toward left edge of the container, unless that doesn’t make sense with the flex-direction, then it behaves like start.  
- __*right*__ : items are packed toward right edge of the container, unless that doesn’t make sense with the flex-direction, then it behaves like start.  
- __*center*__ : items are centered along the line  
- __*space-between*__ : items are evenly distributed in the line; first item is on the start line, last item on the end line.  
- __*space-around*__ : items are evenly distributed in the line with equal space around them. Note that visually the spaces aren’t equal, since all the items have equal space on both sides. The first item will have one unit of space against the container edge, but two units of space between the next item because that next item has its own spacing that applies.  
- __*space-evenly*__ : items are distributed so that the spacing between any two items (and the space to the edges) is equal.  

