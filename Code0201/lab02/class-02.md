Headings

HTML has six "levels" of
headings:
<h1> is used for main headings
<h2> is used for subheadings
If there are further sections
under the subheadings then the
<h3> element is used, and so
on...
Browsers display the contents of
headings at different sizes. The
contents of an <h1> element is
the largest, and the contents of
an <h6> element is the smallest.
The exact size at which each
browser shows the headings
can vary slightly. Users can also
adjust the size of text in their
browser. You will see how to
control the size of text, its color,
and the fonts used when we
come to look at CSS.

Paragraphs

To create a paragraph, surround
the words that make up the
paragraph with an opening <p>
tag and closing </p> tag.
By default, a browser will show
each paragraph on a new line
with some space between it and
any subsequent paragraphs.

Bold & Italic

By enclosing words in the tags
<b> and </b> we can make
characters appear bold.
The <b> element also represents
a section of text that would be
presented in a visually different
way (for example key words in a
paragraph) although the use of
the <b> element does not imply
any additional meaning.

Superscript & Subscript


The <sup> element is used
to contain characters that
should be superscript such
as the suffixes of dates or
mathematical concepts like
raising a number to a power such
as 22.

The <sub> element is used to
contain characters that should
be subscript. It is commonly
used with foot notes or chemical
formulas such as H20.

White Space

In order to make code easier to
read, web page authors often
add extra spaces or start some
elements on new lines.
When the browser comes across
two or more spaces next to each
other, it only displays one space.
Similarly if it comes across a line
break, it treats that as a single
space too. This is known as
white space collapsing.
You will often see that web page
authors take advantage of white
space collapsing to indent their
code in order to make it easier
to follow.

Line Breaks & Horizontal Rules

As you have already seen, the
browser will automatically show
each new paragraph or heading
on a new line. But if you wanted
to add a line break inside the
middle of a paragraph you can
use the line break tag <br />.

To create a break between
themes — such as a change of
topic in a book or a new scene
in a play — you can add a
horizontal rule between sections
using the <hr /> tag.
There are a few elements that
do not have any words between
an opening and closing tag. They
are known as empty elements
and they are written differently.
An empty element usually
has only one tag. Before the
closing angled bracket of an
empty element there will often
be a space and a forward slash
character. Some web page
authors miss this out but it is a
good habit to get into.

Strong & Emphasis

<strong>
The use of the <strong>
element indicates that its
content has strong importance.
For example, the words
contained in this element might
be said with strong emphasis.
By default, browsers will show
the contents of a <strong>
element in bold.

<em>
The <em> element indicates
emphasis that subtly changes
the meaning of a sentence.
By default browsers will show
the contents of an <em> element
in italic.

Abbreviations &
Acronyms

<abbr> html HTML
If you use an abbreviation or
an acronym, then the <abbr>
element can be used. A title
attribute on the opening tag is
used to specify the full term.
In HTML 4 there was a separate
<acronym> element for
acronyms. To spell out the full
form of the acronym, the title
attribute was used (as with the
<abbr> element above). HTML5
just uses the <abbr> element
for both abbreviations and
acronyms.

Understanding CSS:
Thinking Insi de the Box

CSS allows you to create rules that control the
way that each individual box (and the contents
of that box) is presented.

CSS Associates Style rules with HTML elements

CSS works by associating rules with HTML elements. These rules govern
how the content of specified elements should be displayed. A CSS rule
contains two parts: a selector and a declaration

CSS Properties Affect How Elements Are Displayed

CSS declarations sit inside curly brackets and each is made up of two
parts: a property and a value, separated by a colon. You can specify
several properties in one declaration, each separated by a semi-colon.

<link> external-css.html HTML
The <link> element can be used
in an HTML document to tell the
browser where to find the CSS
file used to style the page. It is an
empty element (meaning it does
not need a closing tag), and it
lives inside the <head> element.
It should use three attributes:

href
This specifies the path to the
CSS file (which is often placed in
a folder called css or styles).


type
This attribute specifies the type
of document being linked to. The
value should be text/css.


rel
This specifies the relationship
between the HTML page and
the file it is linked to. The value
should be stylesheet when
linking to a CSS file.
An HTML page can use more
than one CSS style sheet. To
do this it could have a <link>
element for every CSS file it
uses. For example, some authors
use one CSS file to control the
presentation (such as fonts and
colors) and a second to control
the layout.


*style*
You can also include CSS rules
within an HTML page by placing
them inside a *style* element,
which usually sits inside the
*head* element of the page.
The *style* element should use
the type attribute to indicate
that the styles are specified in
CSS. The value should be text/
css.
When building a site with more
than one page, you should use
an external CSS style sheet. This:
●● Allows all pages to use the
same style rules (rather than
repeating them in each page).
●● Keeps the content separate
from how the page looks.
●● Means you can change the
styles used across all pages
by altering just one file
(rather than each individual
page).

PLACING THE SCRIPT
IN THE PAGE

It is best to keep JavaScript code in its own JavaScript
file. JavaScript files are text files (like HTML pages and
CSS style sheets), but they have the . j s extension.
The HTML <script> element is used in HTML pages
to tell the browser to load the JavaScript file (rather like
the <link> element can be used to load a CSS file).
If you view the source code of the page in the browser,
the JavaScript will not have changed the HTML,
because the script works with the model of the web
page that the browser has created.

