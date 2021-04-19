<img src = "https://www.otallu.com/wp-content/uploads/2017/08/basic-html-layout-tutorial-image.jpg">

# Layout

## Key Concepts in Positioning Elements

### Building Blocks

CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.

Block-level boxes start on a new line and act as the main building blocks of any layout, while inline boxes flow between surrounding text. You can control how much space each box takes up by setting the width of the boxes (and sometimes the height, too). To separate boxes, you can use borders, margins, padding, and background colors.

**Block-level elements** : start on a new line

**Inline elements** : flow in between surrounding text

### Containing Elements

If one block-level element sits inside another
block-level element then the outer box is
known as the containing or parent element.

It is common to group a number of elements together inside a (div) (or other block-level) element. For example, you might group together all of the elements that form the header of a site (such as the logo and the main navigation). The (div) element that contains this group of elements is then referred to as the containing element.

## Controlling the Position of Elements

CSS has the following positioning schemes that allow you to control the layout of a page: normal flow, relative positioning, and absolute positioning. You specify the positioning scheme using the positionproperty in CSS. You can also float elements using the float property.

* Normal flow

Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one Even if you specify the width of the boxes and there is space for two elements to sit side-byside, they will not appear next to each other. This is the default behavior (unless you tell the browser to do something else).

* Relative Positioning

This moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed. This does not affect the position of surrounding elements; they stay in the position they would be in in normal flow.

* Absolute positioning

This positions the element in relation to its containing element. It is taken out of normal flow, meaning that it does not affect the position of any surrounding elements (as they simply ignore the space it would have taken up). Absolutely positioned elements move as users scroll up and down the page.


To indicate where a box should be positioned, you may also need to use box offset properties to tell the browser how far from the top or bottom and left or right it should be placed. (You will meet these when we introduce the positioning schemes on the following pages.)

* Fixed Positioning 

This is a form of absolute positioning that positions the element in relation to the browser window, as opposed to the containing element. Elements with fixed positioning do not affect the position of surrounding elements and they do not move when the user scrolls up or down the page.

* Floating Elements

Floating an element allows you to take that element out of normal flow and position it to the far left or right of a containing box. The floated element becomes a block-level element around which other content can flow.

When you move any element from normal flow, boxes can overlap. The z-index property allows you to control which box appears on top.

## Clearing Floats

The clear property allows you to say that no element (within the same containing element) should touch the left or righthand sides of a box. It can take the following values:

* **left**

The left-hand side of the box should not touch any other elements appearing in the same containing element.

* **right**

The right-hand side of the box will not touch elements appearing in the same containing element.

* **both**

Neither the left nor right-hand sides of the box will touch elements appearing in the same containing element.

* **none**

Elements can touch either side.

## Creating Multi-Column Layouts with Floats

Many web pages use multiple columns in their design. This is achieved by using a (div) element to represent each column. The following three CSS properties are used to position the columns next to each other:

* **width**

This sets the width of the columns.

* **float**

This positions the columns next to each other.

* **margin**

This creates a gap between the columns.

## Fixed Width Layouts

Fixed width layout  designs do not change size as the user increases or decreases the size of their browser window. Measurements tend to be given in pixels.

**Advantages**

● Pixel values are accurate at controlling size and positioning of elements.

● The designer has far greater control over the appearance and position of items on the page than with liquid layouts.

● You can control the lengths of lines of text regardless of the size of the user's window.

● The size of an image will always remain the same relative to the rest of the page.

**Disadvantages**

● You can end up with big gaps around the edge of a page.

● If the user's screen is a much higher resolution than the designer's screen, the page can look smaller and text can be harder to read.

● If a user increases font sizes, text might not fit into the allotted spaces.

● The design works best on devices that have a site or resolution similar to that of desktop or laptop computers.

● The page will often take up more vertical space than a liquid layout with the same content.

## Summary

* (div) elements are often used as containing elements to group together sections of a page.

* Browsers display pages in normal flow unless you specify relative, absolute, or fixed positioning.

* The float property moves content to the left or right of the page and can be used to create multi-column layouts. (Floated items require a defined width.)

* Pages can be fixed width or liquid (stretchy) layouts.

* Designers keep pages within 960-1000 pixels wide, and indicate what the site is about within the top 600 pixels (to demonstrate its relevance without scrolling).

* Grids help create professional and flexible designs.

* CSS Frameworks provide rules for common tasks.

* You can include multiple CSS files in one page.

# THE END
