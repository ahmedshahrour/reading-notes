Controlling the Position of Elements

CSS has the following positioning schemes that allow you to control
the layout of a page: normal flow, relative positioning, and absolute
positioning. You specify the positioning scheme using the position
property in CSS. You can also float elements using the float property.

Normal flow
Every block-level element
appears on a new line, causing
each item to appear lower down
the page than the previous one.
Even if you specify the width
of the boxes and there is space
for two elements to sit side-byside,
they will not appear next
to each other. This is the default
behavior (unless you tell the
browser to do something else).

Relative Positioning
This moves an element from the
position it would be in normal
flow, shifting it to the top, right,
bottom, or left of where it
would have been placed. This
does not affect the position of
surrounding elements; they stay
in the position they would be in
in normal flow.

Absolute positioning
This positions the element
in relation to its containing
element. It is taken out of
normal flow, meaning that it
does not affect the position
of any surrounding elements
(as they simply ignore the
space it would have taken up).
Absolutely positioned elements
move as users scroll up and
down the page.

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

position:static

In normal flow, each block-level
element sits on top of the next
one. Since this is the default
way in which browsers treat
HTML elements, you do not
need a CSS property to indicate
that elements should appear
in normal flow, but the syntax
would be:
position: static;
I have not specified a width
property for the heading
element, so you can see how it
stretches the width of the entire
browser window by default.
The paragraphs are restricted
to 450 pixels wide. This shows
how the elements in normal flow
start on a new line even if they
do not take up the full width of
the browser window.

position:absolute

When the position property
is given a value of absolute,
the box is taken out of normal
flow and no longer affects the
position of other elements on
the page. (They act like it is not
there.)
The box offset properties (top
or bottom and left or right)
specify where the element
should appear in relation to its
containing element.
In this example, the heading has
been positioned at the top of the
page and 500 pixels from its left
edge. The width of the heading is
set to be 250 pixels wide.
The width property has
also been applied to the <p>
elements in this example
to prevent the text from
overlapping and becoming
unreadable.

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

using float to place Elements Side-by-Side

A lot of layouts place boxes
next to each other. The float
property is commonly used to
achieve this.
When elements are floated, the
height of the boxes can affect
where the following elements sit.
In this example, you can see six
paragraphs, each of which has a
width and a float property set.
The fourth paragraph does not
go across to the left hand edge
of the page as one might expect.
Rather it sits right under the
third paragraph.
The reason for this is that the
fourth paragraph has space to
start under the third paragraph,
but it cannot go any further to
the left because the second
paragraph is in the way.

creating Multi-Column Layouts with Floats

Many web pages use multiple
columns in their design. This
is achieved by using a <div>
element to represent each
column. The following three CSS
properties are used to position
the columns next to each other:
width This sets the width of the
columns.
float
This positions the columns next
to each other.
margin
This creates a gap between the
columns.
A two-column layout like the one
shown on this page would need
two <div> elements, one for the
main content of the page and
one for the sidebar.