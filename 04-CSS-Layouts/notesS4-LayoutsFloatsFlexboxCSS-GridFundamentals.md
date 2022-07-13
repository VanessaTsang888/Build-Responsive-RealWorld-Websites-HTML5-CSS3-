45. Section Intro:

Up until this point we used css to add visual styles ad spacing to elements. However, css is used mainly to build layouts. We now learn to use css
to build layouts using floats and also using two really modern technologies called Flexbox and CSS Grids.

46. The 3 Ways of Building Layouts:
    Arranging elements in to some kind of structure.

There are 2 types of layouts: Page Layout vs. Component Layout.

1. Page layout is what we've been learning - laying out element or conent inside of a website.
2. On the other hand, some elements are made up of components and these need some kind of layout too as they are made up of smaller pieces of content that need
   to be arranged in some kind of way. So components themseleves also have a layout.

Float Layouts:
The old way of building layouts of all sizes, using the flat css property. Still used, but getting outdated fast.

Flexbox:
Modern way of laying out elements in a 1-dimensional row without using floats. Perfect for component layouts.

CSS Grid:s
Another modern way for laying out element in a fully-fledged 2-dimentsional grid. Perfect for page layouts and complex components.

47. Using Floats:
    I've already learnt this in the past. Will come back to this for a refresher at the end.

To make elements appear side-by-side.

Colapsing height.

48. Clearing Floats:

The h1 element colapsed its height as all its child elements are floated. Therefore we need to use clear the float.

To clear float:
The clear fix hack will avoid having empty div's.

- Add a clearfix class in the header/parent element. Use that in css code and use the after sudo element this will create a new element, which will be the last child element of the container. This is similar to adding the empty div manually. Needs content. Set from inline to block element.

50: Box-sizing: border-box:

How we can run into problems with the default box model and how we can fix it.
Example, currently the side bar has no margin on the right and no padding on the left.
The default padding is 50 40. But our element for the aside is 300 x 463. So it don't fit and moves down as on the left is the article which is width 825px. To fix this issue:

1. Leave behind how the default box model works and look at the other box model:
   -> property: box-sizing
   -> value: border-box
2. The default is whenever we specify a height or a width, then the box model will add the border and padding on top of that. This is the problem in our example aside that moved down the bottom as it no longer fit next to the article.
   So we want to define the width and height then the element will be exactly that size no matter what border or padding. We do this by adding the property
   box-sizing and the value of border-box:
   aside {
   background-color: red;
   width: 300px;
   float: right;
   /_ This should be applied to every element. _/
   box-sizing: border-box;
   }

51: Challenge #1:
Contiue with the shoe challenge.

52: Intro to Flexbox:

The main idea behind flexbox is that empty space inside a container element can be automatically divded by its child elements.
Flexbox makes it easy to automatically align items to one another inside a parent container, both horizontally and vertically.
Flexbox solves common problems such as vertical centering and creating equal-heigh columns.
Flexbox is perfet for replacing floats, allowing us to write fewer and cleaner HTML and CSS code, so easier to maintain and less bugs.

1.  The Flex container:
    Just set its property to flex: display: flex;
    Then all its direct children of that contain will become flex-items. Use different properties on flex contain and flex items.

2.  The Main Axis and the Cross Axis. We can change these if we wish.
    The Box Model with Box-Sizing: Border-Box:
    Apply to article element, better still put within the Universal Selector at the top of the file.

- {
  /_ border-top: 10px solid #1098ad; _/
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  }

55. The flex Property:
    I've made notes in my CSS dictionary.

56. Adding Flexbox to Our Project:
    I've watched the video but not code with the instructor as yet.

57. Building a Simple Flexbox Layout:
    Continue from here.

58. Intro to CSS Grid:
    very powerful compared to floats and flexbox.
    The most complete and easiest way of building layouts. Setting up a simple grid take less than a minuet.
    Use to define our 2-D layout - our column and our rows.

           Just like flexbox the element stretch across the entire cell, across the height and width.

59. A CSS Grid Overview:
