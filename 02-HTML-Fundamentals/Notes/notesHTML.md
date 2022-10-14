SECTION 2: HTML Fundamentals:

L9 Section Intro:
Will build an example project to learn html i.e. headings, paragraphs, links etc.

HTML BASIC: Div into HTML:
L10 Intro to HTML.
What is html and what we can do with it?

-> HyperText Markup Language.
One of the corse web technologies alone with CSS and JavaScript.
HTML is a markp language that web devs can use to structure and describe the content of a webpage - not a programming language.
-> HTML consists of elements that describe different types of content: paragraphs, links, headings, images, videos etc. So we use elements to describe content.
-> Web browsers understand HTML and reder HTML code as websites.

The anatomy or the building blocks of each HTML element:

<p> HTML is a markup language</p>
The whole of this is the element itself. Made of 3 parts: the opening tag, the content, the closing tag.

L11: HTML Document Structure:
A structure each HTML doc needs to have.

The Project:
The code magazine which is a blog post.
1 - create html basic structure;
2 - see the index.htl file in this section.

L12: Text Elements:
Working with text, how to markup text.
Headings:
To break up big blocks of text, add a title to each of the sections. There are 6 different headings so we can establish a hierarchy in our text so we can go from
h1 to h6.
Example:

<h1>The Code Magazine</h1>
<h2>The Basic Language of the Wb: HTML</h2>
<h3>What is HTML?</h3>

Italic bold:
Use <strong></strong> to make text bold from HTML5 not <b></b>

Make text italic:
Make the word fundamentals italic:
use the <em></em> element for emphasize NOT the <i></i>

Challenge:
Make the first letter of 'HyperText Markup Language' bold.
I used the <strong></strong> element to do that.

L13: More Text ElementsL Lists:
How to create lists with bullet points and numbers.

Each element has a meaning and we need them to structure our content. We use elements to give our content some meaning.
HTML don't care about any white space.

L14: Images and Attributes:
Currently my blog post is missing images using the HTML image element.
the alt (alternative text) attribute - some text to describe what the image is about.
This allows Chrome to know what is in the image.

By specifying the description of the image we can also allow blind people to use our website or user who use a screen reader will not see our images but their screen reader will read the alternative text to them. Therefore important to write a good description.

Challenge:
To include the luara joines image below the h2 element, 50px for the width and height.

We can use attributes to specify character sets that go in to our document, i.e. the meta data. Use all the simple characters in the English language: <meta charset="UTF-8" />

L15: Hyperlinks or anchor links:
Allows the internet to be world wide web. Links between pages.
Links that point to other pages within our own website:
Links that point to other websites/pages outside of our website: use the target attribute. This will allow users to open it in new tab whilst the original one is still open.
Example:

<p>
You can learn more at the
<a
        href="https://developer.mozilla.org/en-US/docs/Web/HTML"
        target="_blank"
        >MDN Web Docs</a
      >.
</p>

What makes the anchor element a link is the href property. If we don't want it to point to anywhere then we specify a hash symbol - a placeholder link.

L16: Structuring Our Page:
For Semantic HTML:
To markup/describe our content.
Time to add some structure to our document and to our elements using the new HTML5 elements.
At the moment our elements are not grouped together in any logical way. So we need container elements to group our current elements together:

Links -> use page navigation: <nav></nav> element. I've used this nav container element to group all 4 links under the h1 element. In the UI nothing has changed which is what I expect.
Group the h1 and navigation links inside of a Header element as the rest of the content is the Blog itself: <header></header> for the top part of our page.

For the rest of the content and its elements which is the blog post itslef we can use the <article></article> container element which is very common.
Now our body element only have 2 direct child elements, the <header> and the <article>.

Now do some grouping inside of the <article></article> element.
Inside of <article></article> we can use the <header> element to group the h2, image, paragraph and post img together.

The footer:

<footer> for the copyright text.

L17: A Note on Semantic HTML:
Before HTML5 most people used <div> most of the time. Now with HTML5, we write semantic HTML.

<div> is just  container.
Elements and container elements have meaning, i.e. <nav></nav> contain element is used to group a bunch of navigation links which is important for browsers to understand what the elements are, important for SEO and accessibility - especially for people with screen readers to consue on web pages.
Using elements may not change anything on the UI but need to understand what these elements means and what they stand for.
Summary:
1 -> for broswers to understand our elements/web pages;
2 - for SEO / optimiseation;
3 - for accessibility, i.e. people with screen readers.

L18 Installing aAdditional VS Code Extensions:
Three others to make our life easier when we code HTML and CSS.

1 - Image Previous - displays small image in gutter. Can be extremely helpful sometimes.
2 - Color Hightlight - helpfull when visualising colors in CSS.
3 - Auto Rename Tag - when I change the opening tag, it will auto change the closing one for me. Will this work for React? I will try this out when I get to my React personal development.

Go to Settings and enable the Auto Closing Tag. I've check and found that I've already done this. So when I write the opening <p> HTML is auto write the closing tag for me.

4 - Live Server: I have already download this from a previous course/project. I have the 'Go Live' button on bottom-right. It will open new tab which will contain my web page. It will auto reload my web page in the UI when I make a change to my code and save it.
On save, page will get auto updated. To stop the connection, click the Port: 5500 icon at the bottom. The port is the first couple of digits on the url. I have my own web server on my own computer running. The port is the address of my web server or the local host server.

L19 Code Challenge 01:
