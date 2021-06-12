Height & Width of Images

height
This specifies the height of the
image in pixels.
width
This specifies the width of the
image in pixels.
Images often take longer to
load than the HTML code that
makes up the rest of the page.
It is, therefore, a good idea to
specify the size of the image
so that the browser can render
the rest of the text on the page
while leaving the right amount of
space for the image that is still
loading.
The size of images is increasingly
being specified using CSS rather
than HTML — see pages 409-
410 for more information about
this.

Aligning Images Horizontally

align horizontally.html HTML
The align attribute was
commonly used to indicate how
the other parts of a page should
flow around an image. It has
been removed from HTML5
and new websites should use
CSS to control the alignment of
images (as you will see on pages
411-412).
I have discussed it here because
you are likely to come across
it if you look at older code, and
because some visual editors still
insert this attribute when you
indicate how an image should be
aligned.
The align attribute can take
these horizontal values:
left
This aligns the image to the left
(allowing text to flow around its
right-hand side).
right
This aligns the image to the right
(allowing text to flow around its
left-hand side).

Aligning Images Vertic ally

As you saw on the last page, the
align attribute is no longer used
in HTML5, but it is covered here
because you may see it used in
older websites and it is still used
in the code created by some
visual editors.
You can see how to use CSS
to achieve the same effects on
pages 285-286.
There are three values that the
align attribute can take that
control how the image should
align vertically with the text that
surrounds it:
top
This aligns the first line of the
surrounding text with the top of
the image.
middle
This aligns the first line of the
surrounding text with the middle
of the image.
bottom
This aligns the first line of the
surrounding text with the bottom
of the image.


Claas Attribute 

Every HTML element can
also carry a class attribute.
Sometimes, rather than uniquely
identifying one element within
a document, you will want a
way to identify several elements
as being different from the
other elements on the page.
For example, you might have
some paragraphs of text that
contain information that is more
important than others and want
to distinguish these elements, or
you might want to differentiate
between links that point to other
pages on your own site and links
that point to external sites.
To do this you can use the
class attribute. Its value
should describe the class it
belongs to. In the example on
the left, key paragraphs have a
class attribute whose value is
important.
The class attribute on any
element can share the same
value. So, in this example, the
value of important could be
used on headings and links, too.

Inline elements
Some elements will always
appear to continue on the
same line as their neighbouring
elements. These are known as
inline elements.

Grouping Text &
Elements In a Block

<div> block-elements.html HTML
The <div> element allows you to
group a set of elements together
in one block-level box.
For example, you might create
a <div> element to contain all
of the elements for the header
of your site (the logo and the
navigation), or you might create
a <div> element to contain
comments from visitors.
In a browser, the contents of
the <div> element will start on
a new line, but other than this
it will make no difference to the
presentation of the page.
Using an id or class attribute
on the <div> element, however,
means that you can create
CSS style rules to indicate how
much space the <div> element
should occupy on the screen and
change the appearance of all the
elements contained within it.
It can also make it easier to
follow your code if you have used
<div> elements to hold each
section of the page.

Grouping Te xt &
Elements Inline

<span>
The <span> element acts like
an inline equivalent of the <div>
element. It is used to either:
1. Contain a section of text
where there is no other suitable
element to differentiate it from
its surrounding text
2. Contain a number of inline
elements
The most common reason why
people use <span> elements
is so that they can control the
appearance of the content of
these elements using CSS.
You will usually see that a class
or id attribute is used with
<span> elements:
●● To explain the purpose of this
<span> element
●● So that CSS styles can be
applied to elements that
have specific values for these
attributes

IFrames

<iframe> 08/iframes.html HTML
An iframe is like a little window
that has been cut into your
page — and in that window you
can see another page. The term
iframe is an abbreviation of inline
frame.
One common use of iframes
(that you may have seen on
various websites) is to embed
a Google Map into a page. The
content of the iframe can be any
html page (either located on the
same server or anywhere else on
the web).
An iframe is created using the
<iframe> element. There are a
few attributes that you will need
to know to use it:
src
The src attribute specifies the
URL of the page to show in the
frame.
height
The height attribute specifies
the height of the iframe in pixels.
width
The width attribute specifies
the width of the iframe in pixels.




