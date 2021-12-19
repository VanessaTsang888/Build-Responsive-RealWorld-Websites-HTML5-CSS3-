I already know most of this but will recap on some of the lectures on this section 3: CSS Fundamentals.

25. Combining Selectors:

if all heading uses same font family then create a list of selectors in order to select multiple elments then apply the font family to that list. So when we need to change
the font then we only need to do it in one place. continue from 1:10

28. Pseudo-classes:
Example, style the first list elements from two different lists differently -> first element from each list should be bold. One way is to add a class to each list item: -> <li class="first-li"></li>
    -> css - select all elements with all li class -> .first-li { font-weight: bold; }

Example 2: instead of doing it mannual we can get css auto figure out which is the first 'li' element inside of a container using a Pseudo-class which is using a colon as below:
-> li: first-child { font-weight: bold }
So we changed our selector and added a Pseudo-classes. What the first-child Pseudo-classes does is it will select all the li elements that are the
first child elements of its parent elements the <ol> element. Another example of using Pseudo-classes but to select the last list item from all lists:
-> li:last-child { font-style: italic; }
We can also target a specific child, i.e. the third or second child using the nth-child Pseudo-classes
-> i.e. we want the second child to have a color of red:
-> li:nth-child(2) {
    color: red;
}

continue from: 5:50


41. Pseudo-elements: How to work with Pseudo-elements in HTML:
A css feature. A Pseudo-elements is written with two colons.
Elements that don't exist in the html but we can still style in css, i.e. the first letter of a paragraph or the first line of a paragraph. Use a first letter Pseudo-elements to target the first letter of a paragraph. We want the first letter within the h1 to be normal as in not italic and we want some space to the right of that:
-> h1::first-letter { font-style: normal; margin-right: 5px }

Pseudo-elements can work with emojis as well.

To select the first line in each paragraph and style it red:
-> p::first-line { color: red; }

Only select the paragraphs that come after the h3:
-> h3 + p::first-line { color: red; }

The before and after Pseudo-elements:
The below content don't exist in our html, only in our Dev Tools.
-> h2::after { content: "TOP"; color: black; font-size: 16px; padding: 5px 10 px; position: absolute; top: -10px; right: -25px }
