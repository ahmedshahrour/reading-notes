  Storing Images on Your Site

  As a website grows, keeping
images in a separate folder
helps you understand how the
site is organized. Here you can
see an example of the files for
a website; all of the images are
stored in a folder called images.
On a big site you might like to
add subfolders inside the images
folder. For example, images such
as logos and buttons might sit in
a folder called interface, product
photographs might sit in a page
called products, and images
related to news might live in a
folder called news.
If you are using a content
management system or blogging
platform, there are usually tools
built into the admin site that
allow you to upload images,
and the program will probably
already have a separate folder
for image files and any
other uploads.


Adding Images

<img> images.html HTML
To add an image into the page
you need to use an <img>
element. This is an empty
element (which means there is
no closing tag). It must carry the
following two attributes:
src
This tells the browser where
it can find the image file. This
will usually be a relative URL
pointing to an image on your
own site. (Here you can see that
the images are in a child folder
called images — relative URLs
were covered on pages 83-84).
alt
This provides a text description
of the image which describes the
image if you cannot see it.
title
You can also use the title
attribute with the <img> element
to provide additional information
about the image. Most browsers
will display the content of this
attribute in a tootip when the
user hovers over the image.

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

Old Code: Aligning Images Vertic all


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

HTML5: Figure and Figure Caption

<figure>
Images often come with
captions. HTML5 has introduced
a new <figure> element to
contain images and their caption
so that the two are associated.
You can have more than one
image inside the <figure>
element as long as they all share
the same caption.
<figcaption>
The <figcaption> element has
been added to HTML5 in order
to allow web page authors to add
a caption to an image.
Before these elements were
created there was no way to
associate an <img> element with
its caption.
Older browsers that do not
understand HTML5 elements
simply ignore the new elements
and display the content of them.


Foreground Color
color

The color property allows you
to specify the color of text inside
an element. You can specify any
color in CSS in one of three ways:
rgb values
These express colors in terms
of how much red, green and
blue are used to make it up. For
example: rgb(100,100,90)
hex codes
These are six-digit codes that
represent the amount of red,
green and blue in a color,
preceded by a pound or hash #
sign. For example: #ee3e80
color names
There are 147 predefined color
names that are recognized
by browsers. For example:
DarkCyan
We look at these three different
ways of specifying colors on the
next double-page spread.
CSS3 has also introduced
another way to specify colors
called HSLA.

Background Color

CSS treats each HTML element
as if it appears in a box, and the
background-color property
sets the color of the background
for that box.
You can specify your choice of
background color in the same
three ways you can specify
foreground colors: RGB values,
hex codes, and color names
(covered on the next page).
If you do not specify a
background color, then the
background is transparent.
By default, most browser
windows have a white
background, but browser users
can set a background color for
their windows, so if you want
to be sure that the background
is white you can use the
background-color property on
the <body> element.



CSS 3: Opacity

CSS3 introduces the opacity
property which allows you to
specify the opacity of an element
and any of its child elements.
The value is a number between
0.0 and 1.0 (so a value of 0.5
is 50% opacity and 0.15 is 15%
opacity).
The CSS3 rgba property allows
you to specify a color, just like
you would with an RGB value,
but adds a fourth value to
indicate opacity. This value is
known as an alpha value and is
a number between 0.0 and 1.0
(so a value of 0.5 is 50% opacity
and 0.15 is 15% opacity). The
rgba value will only affect the
element on which it is applied
(not child elements).
Because some browsers will
not recognize RGBA colors, you
can offer a fallback so that they
display a solid color. If there are
two rules that apply to the same
element, the latter of the two
will take priority. To create the
fallback, you can specify a color
as a hex code, color name or
RGB value, followed by the rule
that specifies an RGBA value. If
the browser understands RGBA
colors it will use that rule. If it
doesn't, it will use the RGB value.
At the time of writing, the
opacity and rgba properties
are only supported by the most
recent browsers.


CSS 3: HSL Colors

CSS3 introduces an entirely new and intuitive
way to specify colors using hue, saturation,
and lightness values.

Techniques That Offer a Wider Choice of Typefaces


There are several ways to use fonts other than those listed on the
previous page. However, typefaces are subject to copyright, so the
techniques you can choose from are limited by their respective licenses


Specifying Typefaces


The font-family property
allows you to specify the
typeface that should be used for
any text inside the element(s) to
which a CSS rule applies.
The value of this property is the
name of the typeface you want
to use.
The people who are visiting
your site need the typeface you
have specified installed on their
computer in order for it to be
displayed.
You can specify a list of fonts
separated by commas so that,
if the user does not have your
first choice of typeface installed,
the browser can try to use an
alternative font from the list.
It is also common to end with a
generic font name for that type
of font (which you saw on pages
269-270).
If a font name is made up of
more than one word, it should be
put in double quotes.
Designers suggest pages usually
look better if they use no more
than three typefaces on a page.

Size of Type

The font-size property enables
you to specify a size for the
font. There are several ways to
specify the size of a font. The
most common are:
pixels
Pixels are commonly used
because they allow web
designers very precise control
over how much space their text
takes up. The number of pixels is
followed by the letters px.
percentages
The default size of text in
browsers is 16px. So a size of
75% would be the equivalent of
12px, and 200% would be 32px.
If you create a rule to make all
text inside the <body> element
to be 75% of the default size (to
make it 12px), and then specify
another rule that indicates the
content of an element inside the
<body> element should be 75%
size, it will be 9px (75% of the
12px font size).
ems


Leading line-height

Leading (pronounced ledding) is
a term typographers use for the
vertical space between lines of
text. In a typeface, the part of
a letter that drops beneath the
baseline is called a descender,
while the highest point of a letter
is called the ascender. Leading
is measured from the bottom of
the descender on one line to the
top of the ascender on the next.

Letter & Word Spacing

Kerning is the term
typographers use for the space
between each letter. You can
control the space between each
letter with the letter-spacing
property.
It is particularly helpful to
increase the kerning when
your heading or sentence is
all in uppercase. If your text is
in sentence (or normal) case,
increasing or decreasing the
kerning can make it harder to
read.
You can also control the gap
between words using the
word-spacing property.
When you specify a value for
these properties, it should
be given in ems, and it will be
added on top of the default value
specified by the font.
The default gap between
words is set by the typeface
(often around 0.25em), and
it is unlikely that you would
need to change this property
regularly. If the typeface is bold
or you have increased the space
between letters, then a larger
gap between words can increase
readability.

Styling links :

Browsers tend to show links
in blue with an underline by
default, and they will change
the color of links that have been
visited to help users know which
pages they have been to.
In CSS, there are two pseudoclasses
that allow you to set
different styles for links that
have and have not yet been
visited.
:link
This allows you to set styles
for links that have not yet been
visited.
:visited
This allows you to set styles for
links that have been clicked on.
They are commonly used to
control colors of the links and
also whether they are to appear
underlined or not.
On the left, you can see that
visited links are shown in a
different color to help visitors
know what they have already
seen.
Often, the :hover and :active
pseudo-classes (covered on the
next page) are used to alter the
appearance of a link when a user
hovers over or clicks on it.