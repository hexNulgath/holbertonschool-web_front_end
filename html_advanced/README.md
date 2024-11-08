Doctype
The <doctype> is necessary at the top of every HTML page to force the browser to render the page according to relevant specifications.

<!-- Doctype HTML5 -->
<!DOCTYPE html>
<!-- Lowercase is also valid -->
<!doctype html>
Resources
Doctype - MDN Web Docs Glossary: Definitions of Web-related terms | MDN
HEAD - A free guide to head elements
HTML tag
The <html> HTML tag tells the browser that the document is an HTML webpage. It is used as a container for all the HTML elements.

Warning!

The doctype is the only element living outside the html tag.

<html lang="fr" dir="ltr">
Language and reading direction
Building RTL-Aware Web Apps & Websites: Part 1 - Mozilla Hacks - the Web developer blog
head tag
The head tag element contains all the metadatas related to your page. All the elements put in the head are not visible in the window of the browser.

A lot of metadatas exist, some specific to some CMS.

Usage
You can find inside the head:

title of the webpage
asynchronous script calls
metadata
CSS code embed (critical CSS)
JavaScript code embed
Resources
HEAD - A free guide to head elements
Meta charset
The meta charset declares the page’s character encoding.

...
<head>
    <!-- Set character encoding for the document -->
    <meta charset="value">
</head>
...
Resources
meta: The Document-level Metadata element - HTML: Hypertext Markup Language | MDN
Declaring character encodings in HTML
Meta Charset
Viewport
The meta viewport gives information about the initial size of the viewport.

Tip: The viewport is used by mobile devices only.

Accessibility tip: Never use maximum-scale=1.0. It prevents the user from zooming in on the website. It causes an accessibility issue.

...
<head>
    ...
    <!-- Viewport for responsive web design -->
    <meta name="viewport" content="key=value, key=value">
</head>
...
Resources
Responsive Design With Viewport Control
Title
The title meta tag defines the title of the web page.

Tip: The title is only visible on the tab/window of your browser.

Warning! The title should always have less than 56 characters.

...
  <head>
    ...
    <!-- Document Title -->
    <title>Page title</title>
  </head>
...
Resources
The ideal width of the SEO title • Yoast
Meta description
<head>
    ...
    <!-- Meta Description -->
    <meta name="description" content="Description of the page less than 150 characters">
  </head>
Resources
The ideal length of a meta description • Yoast
Favicons
<head>
    ...
    <!-- Standard favicon -->
    <link rel="icon" type="image/x-icon" href="https://example.com/favicon.ico">
    <!-- Recommended favicon format -->
    <link rel="icon" type="image/png" href="https://example.com/favicon.png">
    ...
  </head>
Resources
Favicon & App Icon Generator
Favicon Generator for all platforms: iOS, Android, PC/Mac…
Obsessive cheat sheet to favicon sizes/types.)
Favicons, Touch Icons, Tile Icons, etc. Which Do You Need? | CSS-Tricks
PNG favicons - caniuse
Tag attributes
Attributes provide additional information or instruction for an HTML element. It is always included inside the opening tag.

Data-* attribute
It is possible to declare any attribute using the data- prefix

<tag data-extra-attr="value">some content</tag>
Resources
HTML attribute reference - HTML: Hypertext Markup Language | MDN
header tag
The <header> HTML tag element is used to identify the top of a webpage, article, section, or other segment of a page. The header is normally always the same across all pages of your website.



Usage
logo of the website
navigation
search form
...
<body>
    <header>This is my header<header/>
</body>
Warning! The main element should never be a descendant of an article, aside, header, footer, or nav element.

Don’t confuse header with the head element of the page.

Resources
header - HTML: Hypertext Markup Language | MDN
main tag
The <main> HTML tag is a structural element located generally between the <header> and the <footer> and contains the content of your web page.



...
<body>
    <header>This is my header</header>
    <main>
        This is where I put my content
    </main>
</body>
footer tag
The <footer> HTML tag is a structural element used to identify the footer of a page, article, or section.



Usage
copyright information
authorship information
navigation elements
social icons or links
...
<body>
    <header>This is my header<header/>
    <main>
        This is where I put my content
    </main>
    <footer>This is the footer of my page</footer>
</body>
Resources
footer - HTML: Hypertext Markup Language | MDN
aside tag
The <aside> HTML tag contains additional information related to the main content.



Usage
monthly archives
list of categories
...
<body>
    ...
    <main>
        <section>
            <article>This is my article 1</article>
            <article>This is my article 2</article>
            <article>This is my article 3</article>
        </section>
        <aside>
        </aside>
    </main>
    ...
</body>
section tag
The <section> tag element allows the grouping of related elements. You can usually find a <header> and <footer> attached to a section.



Usage
...
<body>
    ...
    <main>
        <section>This is my section 1</section>
        <section>This is my section 2</section>
        <section>This is my section 3</section>
    </main>
    ...
</body>
Resources
section: The Generic Section element - HTML: Hypertext Markup Language | MDN
article tag
An <article> HTML tag represent a self-contained piece of content which could theoretically be distributed to other websites and platforms as a stand-alone unit.



Usage
blog posts
news articles
product cards
forum posts
...
<body>
    ...
    <main>
        <section>
            <article>This is article 1</article>
            <article>This is article 2</article>
        </section>
    </main>
    ...
</body>
Resources
article: The Article Contents element - HTML: Hypertext Markup Language | MDN
nav tag
The <nav> HTML tag is a structural element with navigation links.



...
<body>
    <header> I'm inside the header
        <nav>
          <!-- This is an example of links -->
          <a href="/">Home</a>
          <a href="/about">About</a>
          <a href="/contact">Contact</a>
          <!-- / -->
        </nav>
    <header/>
    ...
</body>
Resources
nav: The Navigation Section element - HTML: Hypertext Markup Language | MDN
Headings
Headings are used to define a section heading.

Type	Self-closing
Block	No
Warning! Browsers apply different sizes for each heading in their default CSS rules. Keep in mind that HTML is about content and not the styling. Never use an h4 after an h2. For example, always keep a descendant order (h1 > h2 > h3…).

Accessibility tip: Headings are used by voice browser to help navigate through the webpage.

<h1>This is my title level 1</h1>
<h2>This is my title level 2</h2>
...
Tip: Never put the logo or name of your website inside an <h1>. The text inside this tag has to reflect the content of your page. On a homepage, based on the design, you can eventually hide visually your <h1> but it still has to exist in your code.

Resources
h1–h6: The HTML Section Heading elements - HTML: Hypertext Markup Language | MDN
p tag
A <p> HTML tag defines a paragraph of text.

Type	Self-closing
Block	No
Warning! If you need a container to wrap multiple elements, use div instead of p. Only use the paragraph tag if your content could be considered a paragraph of text.

<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
Resources
p: The Paragraph element - HTML: Hypertext Markup Language | MDN
div and span don’t possess any semantic meaning. They are mostly used to define a block (div) of content, or an inline (span) content.

span
A span is a generic inline of content used usually for text that are not inside a paragraph. span should be used as little as possible.

<span>This is my first span</span>
Type	Self-closing
Inline	No
div
A div (stands for “document division”) is a generic block of content used to structure elements in your layout.

<div>This is my first div</div>
Type	Self-closing
Block	No
Comments
Comments allow you to add some information visible for the developer but not for the normal user. Comments are not visible on your page.

<!-- This is a comment about how much I love eggs! -->
Resources
About conditional comments (Internet Explorer) | Microsoft Docs
a tag
Links are inline elements which allow you to navigate from one page / document to another.

Type	Self-closing
Inline	No
There are 3 types of targets:

anchor targets, to navigate within the same page
relative URLs, usually to navigate within the same website
absolute URLs, usually to navigate to another website
<a href="#services">Link</a> <-- anchor target -->
<a href="/blog">Link</a> <-- relative url -->
<a href="https://www.example.com">Link</a> <-- absolute url -->
If you use target=_blank don’t forget to add rel=noopner for security purposes.

Resources
a: The Anchor element - HTML: Hypertext Markup Language | MDN
About rel=noopener
Mailto Links | CSS-Tricks
Future changes in the link attribution (rel)
<div>
  <div>
    <a href="#" rel="noopener" target="_blank">Link open in a new tab</a>
  </div>
  <div>
    <a href="#" rel="sponsored">Paid and sponsored links</a>
  </div>
  <div>
    <a href="#" rel="ugc">User-generated content</a>
  </div>
  <div>
    <a href="#" rel="nofollow">Catch-all for all non-trusted links</a>
  </div>
</div>


Resources
Official Google Webmaster Central Blog: Evolving “nofollow” – new ways to identify the nature of links
How Google’s Nofollow, Sponsored, & UGC Links Impact SEO - Moz
Lists
Lists are used for listing ingredients in a recipe, a series of social icons, etc..

Type	Self-closing
Block	No
Resources
ul: The Unordered List element - HTML: Hypertext Markup Language | MDN
li - HTML: Hypertext Markup Language | MDN
ol: The Ordered List element - HTML: Hypertext Markup Language | MDN
dl: The Description List element - HTML: Hypertext Markup Language | MDN
Ordered list (ol)
An ordered list is rendered as a numbered list.

<!-- an ordered list number -->
<ol>
  <li>List item 1</li>
  <li>List item 2</li>
  <li>List item 3</li>
</ol>
<!-- an ordered list width Roman numerals -->
<ol type="i">
  <li>List item 1</li>
  <li>List item 2</li>
  <li>List item 3</li>
</ol>
Unordered list (ul)
An unordered list is rendered as an unordered list of items.

<!-- flat list -->
<ul>
  <li>First bullet point</li>
  <li>Second bullet point</li>
  <li>Third bullet point</li>
</ul>
<!-- list with a nested list -->
<ul>
  <li>First bullet point</li>
  <li>Second bullet point
    <!-- Nested unorderd lit -->
    <ul>
      <li>First bullet point</li>
      <li>Second bullet point</li>
      <li>Third bullet point</li>
    </ul>
  </li> <!-- Closing li tag -->
  <li>Third bullet point</li>
</ul>
Definition list
A definition list is used to list terms and corresponding definitions.

<dl>
  <dt>Term</dt>
  <dd>Definition of the term</dd>
  <dt>Another term</dt>
  <dd>Another definition of the term</dd>
</dl>
Horizontal rules
An hr is a semantic break that separates different blocks of text.

Self-closing
Yes
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
<hr>
<h2>Section</h2>
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
Resources
hr: The Thematic Break (Horizontal Rule) element - HTML: Hypertext Markup Language | MDN
Line Breaks
Line breaks are used to break the text to multiple lines.

Self-closing
yes
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. <br>
Donec viverra<br>
nec<br>
nulla vitae mollis</p>
Never use line breaks for presentation purpose, to create space between elements in your design. Spacing and layout should only be handled by CSS.

Resources
br: The Line Break element - HTML: Hypertext Markup Language | MDN
Inline quotation
Inline quotes is used for inline text that doesn’t require paragraph breaks.

<p>
  According to Mozilla's website,
  <q cite="https://www.mozilla.org/en-US/about/history/details/">Firefox 1.0 was released in 2004 and became a big success.</q>
</p>
Resources
q: The Inline Quotation element - HTML: Hypertext Markup Language | MDN
Blockquote
A multiline quote is called a blockquote.

Type	Self-closing
Block	No
<!-- DO -->
<blockquote cite="https://tools.ietf.org/html/rfc1149">
  <p>Avian carriers can provide high delay, low
  throughput, and low altitude service.  The
  connection topology is limited to a single
  point-to-point path for each carrier, used with
  standard carriers, but many carriers can be used
  without significant interference with each other,
  outside of early spring.  This is because of the 3D
  ether space available to the carriers, in contrast
  to the 1D ether used by IEEE802.3.  The carriers
  have an intrinsic collision avoidance system, which
  increases availability.</p>
</blockquote>
<!-- DON'T -->
<blockquote>For writing maintainable and scalable HTML documents.</blockquote>
<!-- Blockquote with a cite reference -->
<blockquote>
  <p>People think focus means saying yes to the thing you’ve got to focus on. But that’s not what it means at all. It means saying no to the hundred other good ideas that there are. You have to pick carefully. I’m actually as proud of the things we haven’t done as the things I have done. Innovation is saying no to 1,000 things.
    <cite>Steve Jobs – Apple Worldwide Developers’ Conference, 1997</cite>
  </p>
</blockquote>
Resources
blockquote: The Block Quotation element - HTML: Hypertext Markup Language | MDN
Text/Typography
A long list of HTML tags are used to give semantic meaning to specific text. Each tag is essential to help users and browsers understand the specificity of a certain portion of text. It’s crucial to understand which can be used in which situation.

<em> to indicate stress emphasis.
<i> to indicate text set off from the normal prose (foreign word, technical term…).
<strong> to indicate stronger importance.
<b> to draw attention to specific content (keywords in a summary, product names in a review…).
<small> to represent side-comments or small text (copyright, legal text…).
<del> to represent a text that has been deleted.
<ins> to represent a text that has been inserted.
<s> to render text with a strikethough or a line through it.
<wbr> to specify where the text could have a line-break.
<mark> to indicate relevance, representing text marked or highlighted for reference.
<cite> to mark the name of a work, such as a book, play, or song.
<dfn> to mark the defining instance of a term.
<abbr> to represents an abbreviation or acronyme.
<code> to indicate at short fragment of computer code.
<time> to indicate a specific period in time.
<address> to indicate contact information (person, people or organization).
Warning!

Some tags like <strong> and <b> may look the same visually in your browser. Please remember that HTML is about content, semantics, and not the visual aspect.

<ul>
  <li>
    I <em>really</em> like driving in San Francisco.
  </li>
  <li>
    The term <i>voilier</i> is a french word which mean "sailing ship".
  </li>
  <li>
    <strong>Warning!</strong> This is not a drill!
  </li>
  <li>
    <b>This text is bold.</b>
  </li>
  <li>
    <p>Atomic Habits: An Easy & Proven Way to Build Good Habits & Break Bad Ones <small>(Penguin Group USA) <small>Kindle Edition</small>
by</small> James Clear <small>  (Author)</small></p>
  </li>
  <li>
    <p>I'm silently correcting <del>you're</del> <ins>your</ins> grammar.</p>
  </li>
  <li>
    I received <s>$500</s> $1000 for that job!
  </li>
  <li>
    I want to understand <wbr>what</wbr><wbr>is</wbr><wbr>going</wbr><wbr>on</wbr>!
  </li>
  <li>
    <mark>This whole text should be highlighted in yellow.</mark>
  </li>
  <li>
    <blockquote>
    Any inaccuracies in this index may be explained by the fact that it has been sorted with the help of a computer.<br>
    — from <cite>The Art of Computer Programming</cite> by Donald Knuth
    </blockquote>
  </li>
  <li>
    <p>The <strong>HTML Definition element</strong>
    (<strong><dfn>&lt;dfn&gt;</dfn></strong>) is
    used to indicate the term being defined within the context<br/> of a
    definition phrase or sentence.</p>
  </li>
  <li>
    <p>You are the <abbr title="Cascading Style Sheets">CSS</abbr> of my <abbr title="HyperText Markup Language">HTML</abbr>.</p>
  </li>
  <li>
    <code></code>
  </li>
  <li>
    <pre>
      <code>
        body {
          color: red;
        }
      </code>
    </pre>
  </li>
  <li>
    <time datetime="2019-09-19">Sept 19, 2019</time>
  </li>
  <li>
    <address>
      <a href="mailto:someone@example.com">someone@example.com</a>
    </address>
  </li>
</ul>
Resources
em: The Emphasis element - HTML: Hypertext Markup Language | MDN
i - HTML: Hypertext Markup Language | MDN
strong: The Strong Importance element - HTML: Hypertext Markup Language | MDN
b: The Bring Attention To element - HTML: Hypertext Markup Language | MDN
small: the side comment element - HTML: Hypertext Markup Language | MDN
del: The Deleted Text element - HTML: Hypertext Markup Language | MDN
ins - HTML: Hypertext Markup Language | MDN
s - HTML: Hypertext Markup Language | MDN
wbr - HTML: Hypertext Markup Language | MDN
mark: The Mark Text element - HTML: Hypertext Markup Language | MDN
cite: The Citation element - HTML: Hypertext Markup Language | MDN
dfn: The Definition element - HTML: Hypertext Markup Language | MDN
abbr: The Abbreviation element - HTML: Hypertext Markup Language | MDN
code: The Inline Code element - HTML: Hypertext Markup Language | MDN
time - HTML: Hypertext Markup Language | MDN
address: The Contact Address element - HTML: Hypertext Markup Language | MDN
Tables
A table element is used to wrap tabular content. It uses rows and columns to organize the data.

Accessibility tip: Always use <caption> to help people understand the content of your table.

Anatomy of a table
caption: the title of a table.
thead: groups multiple rows that represents the head of the columns
tbody: groups multiple rows that represents the body of the table
tfoot: groups multiple rows that represents the footer of the table
th: a cell as header of a group of table cells
tr: a row of cells
td: a cell of a table
col attribute: defines a column within a table.
colgroup attribute: defines a group of columns within a table.
<!-- Table with thead, tfoot, and tbody -->
<table>
  <caption>The table</caption>
  <thead>
    <tr>
      <th scope="col">Header content 1</th>
      <th scope="col">Header content 2</th>
      <th scope="col">Header content 3</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">Body content 1</th>
      <td>Body content 2</td>
      <td>Body content 3</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <th scope="row">Footer content 1</th>
      <td>Footer content 2</td>
      <td>Footer content 3</td>
    </tr>
  </tfoot>
</table>
<!-- Table without scope -->
<table>
  <caption>The table</caption>
  <thead>
    <tr>
      <th>Header content 1</th>
      <th>Header content 2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Body content 1</td>
      <td>Body content 2</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>Footer content 1</td>
      <td>Footer content 2</td>
    </tr>
  </tfoot>
</table>
Resources
table: The Table element - HTML: Hypertext Markup Language | MDN
thead: The Table Head element - HTML: Hypertext Markup Language | MDN
tbody: The Table Body element - HTML: Hypertext Markup Language | MDN
tfoot: The Table Foot element - HTML: Hypertext Markup Language | MDN
th - HTML: Hypertext Markup Language | MDN
tr: The Table Row element - HTML: Hypertext Markup Language | MDN
td: The Table Data Cell element - HTML: Hypertext Markup Language | MDN
details tag
The <details> HTML element gives a native way to create something similar to an accordion.

<details>
  <summary>Details</summary>
  Something small enough to escape casual notice.
</details>
Resources
details: The Details disclosure element - HTML: Hypertext Markup Language | MDN
summary: The Disclosure Summary element - HTML: Hypertext Markup Language | MDN
Quick Reminder that Details/Summary is the Easiest Way Ever to Make an Accordion | CSS-Tricks
Image
The image element (<img>) allows us to use images on a website.

Type	Self-closing
Inline	Yes
Accessibility tip: You should always have an alt on your image. With text or without, depending if your image is decorative or not. The alt should describe what is inside your image. Never use the title of your blog post or some similar text.

Tip: Always specify the width and height of the image. It will avoid layout jank during image loading. Chrome and other browsers are working (Firefox already has that functionality) on improving the experience.


<!-- using a url relative to the HTML page -->
<img src="img/dog.jpg" alt="My dog Hugo sitting in the grass." width="300" height="200">
<!-- using an absolute url from another website -->
<img src="http://dogpictures.com/dog.jpg" alt="A placeholder image of a dog." width="300" height="200">
Resources
img: The Image Embed element - HTML: Hypertext Markup Language | MDN
Essential Image
Placeholder generators
https://placebear.com/
https://picsum.photos/
http://placehold.it/
https://www.placecage.com/
Image formats
JPEG, PNG, GIF, SVG and WebP are the most common format of image used on the Web. Each of them has his own particularity and usage. It’s essential to understand these and always ensure that they are optimized to be shown on a webpage.

Support image format
JPEG, GIF, PNG OR SVG - Which should You use?
SVG vs PNG vs JPG: Image Format Pros & Cons | Design Shack
SVGOMG - SVGO’s Missing GUI
Warning! It’s not unusual to find websites that load images with more than 1 MB. It’s obviously not recommended. Nowadays, people browse the web more using a wireless connection and then could be limited in their data package. It’s important to always keep that in mind.

Picture
The <picture> HTML tag is used as a wrapper to combine different sources which provide different versions of an image. (It can also be use to offer different versions for different devices/display.)

<picture>
  <source srcset="/img/logo.webp" type="image/webp">
  <source srcset="/img/logo.jp2" type="image/jp2">
  <img src="/img/logo.jpg">
</picture>
Resources
picture: The Picture element - HTML: Hypertext Markup Language | MDN
Bye raster, hello vector: 3 ways to use SVG easier · Devbridge
video tag
The <video> HTML Tag gives the capability to add a native video player in your HTML.

Accessibility tip: It’s essential to provide an alternative text in case the <video> tag is not supported or the video doesn’t exist anymore.

Avoid using the attribute autoplay and let the user decide if they want to play the video. Of course, for videos used in the background, autoplay and loop will probably be essential.

<video width="640" height="480" src="https://archive.org/download/Popeye_forPresident/Popeye_forPresident_512kb.mp4" controls>
  Sorry, your browser doesn't support HTML5 <code>video</code>, but you can
  download this video from the <a href="https://archive.org/details/Popeye_forPresident" target="_blank">Internet Archive</a>.
</video>
Resources
video: The Video Embed element - HTML: Hypertext Markup Language | MDN
Media formats for HTML audio and video
Can I use… video
audio tag
The audio HTML Tag gives the capability to embed sound content in your HTML.

<!-- single audio file -->
<audio src="/music/audiofile.mp3" controls>
<!-- multiple audio files -->
<audio controls>
  <source src="audiofile.mp3" type="audio/mpeg">
  <source src="audiofile.ogg" type="audio/ogg">
</audio>
Resources
audio: The Embed Audio element
Can I use… audio
iframe tag
An iframe embed an external browsing content in your current HTML page.

Type	Self-closing
Block	No
<iframe
  title="Inline Frame Example"
  width="300"
  height="200"
  src="https://www.google.com/">
  Fallback text for non-supported browsers
</iframe>
Accessibility tip: Always specify a title attribute on your iFrame.

Tip: Use iFrames with parcimony as they can add extra weight to your webpage.

Resources
iframe: The Inline Frame element - HTML: Hypertext Markup Language | MDN
3 Reasons You Should Never Use Iframes