Writing Links

Links are created using the <a> element. Users can click on anything
between the opening <a> tag and the closing </a> tag. You specify
which page you want to link to using the href attribute.


Linking to Other Sites


Links are created using the <a>
element which has an attribute
called href. The value of the
href attribute is the page that
you want people to go to when
they click on the link.
Users can click on anything that
appears between the opening
<a> tag and the closing </a>
tag and will be taken to the page
specified in the href attribute.
When you link to a different
website, the value of the href
attribute will be the full web
address for the site, which is

Directory Structure

Structure
The diagram on the right shows
the directory structure for a
fictional entertainment listings
website called ExampleArts.
The top-level folder is known
as the root folder. (In this
example, the root folder is called
examplearts.) The root folder
contains all of the other files and
folders for a website.
Each section of the site is placed
in a separate folder; this helps
organize the files.

Rela tionships
The relationship between
files and folders on a website
is described using the same
terminology as a family tree.
In the diagram on the right, you
can see some relationships have
been drawn in.
The examplearts folder is a
parent of the movies, music
and theater folders. And the
the movies, music and theater
folders are children of the
examplearts folder.

Homepa ges
The main homepage of a site
written in HTML (and the
homepages of each section in a
child folder) is called index.html.
Web servers are usually set up
to return the index.html file if no
file name is specified.
Therefore, if you enter
examplearts.com it will return
examplearts.com/index
.html, and examplearts.com/
music will return examplearts
.com/music/index.html.

Containing Elements
If one block-level element sits inside another
block-level element then the outer box is
known as the containing or parent element.
It is common to group a number of elements together inside a <div>
(or other block-level) element. For example, you might group together
all of the elements that form the header of a site (such as the logo and
the main navigation). The <div> element that contains this group of
elements is then referred to as the containing element.

To indicate where a box should be positioned, you may also need to use
box offset properties to tell the browser how far from the top or bottom
and left or right it should be placed. (You will meet these when we
introduce the positioning schemes on the following pages.)


Fixed Positioning
This is a form of absolute
positioning that positions
the element in relation to the
browser window, as opposed
to the containing element.
Elements with fixed positioning
do not affect the position of
surrounding elements and they
do not move when the user
scrolls up or down the page.

Floating Elements
Floating an element allows
you to take that element out
of normal flow and position
it to the far left or right of a
containing box. The floated
element becomes a block-level
element around which other
content can flow.


Overlapping Elements

When you use relative, fixed, or
absolute positioning, boxes can
overlap. If boxes do overlap, the
elements that appear later in the
HTML code sit on top of those
that are earlier in the page.
If you want to control which
element sits on top, you can use
the z-index property. Its value
is a number, and the higher the
number the closer that element
is to the front. For example, an
element with a z-index of 10
will appear over the top of one
with a z-index of 5.

Floating Elements

The float property allows you
to take an element in normal
flow and place it as far to the
left or right of the containing
element as possible.
Anything else that sits inside
the containing element will
flow around the element that is
floated.
When you use the float
property, you should also use the
width property to indicate how
wide the floated element should
be. If you do not, results can be
inconsistent but the box is likely
to take up the full width of the
containing element (just like it
would in normal flow).

Clearing Floats

The clear property allows you
to say that no element (within
the same containing element)
should touch the left or righthand
sides of a box. It can take
the following values:
left
The left-hand side of the box
should not touch any other
elements appearing in the same
containing element.
right
The right-hand side of the
box will not touch elements
appearing in the same containing
element.
both
Neither the left nor right-hand
sides of the box will touch
elements appearing in the same
containing element.
none
Elements can touch either side.
In this example, the fourth
paragraph has a class called
clear. The CSS rule for this
class uses the clear property
to indicate that nothing should
touch the left-hand side of it. The
fourth paragraph is therefore
moved further down the page
so no other element touches its
left-hand side.

