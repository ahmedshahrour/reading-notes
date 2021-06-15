Forms 

There are several types of form controls that
you can use to collect information from visitors
to your site.

ADDING TEXT

Used for a single line of text such
as email addresses and names

Password input

Like a single line text box but it
masks the characters entered.

Text area

For longer areas of text, such as
messages and comments.

Making Choices

Radio buttons
For use when a user must select
one of a number of options.

Checkboxes

When a user can select and
unselect one or more options

Drop-down boxes

When a user must pick one of a
number of options from a list.

Submitting Forms:

To submit data from your form
to another web page.

Image buttons

Similar to submit buttons but
they allow you to use an image.

Uploading Files:

Allows users to upload files
(e.g. images) to a website.

A form may have several form controls, each
gathering different information. The server
needs to know which piece of inputted data
corresponds with which form element.

*form*

Form controls live inside a
*form* element. This element
should always carry the action
attribute and will usually have a
method and id attribute too.

action

Every <form> element requires
an action attribute. Its value
is the URL for the page on the
server that will receive the
information in the form when it
is submitted.

method

With the get method, the values
from the form are added to
the end of the URL specified in
the action attribute. The get
method is ideal for:

●● short forms (such as search
boxes)

●● when you are just retrieving
data from the web server
(not sending information that
should be added to or deleted
from a database)

*input*

The <input> element is used
to create several different form
controls. The value of the type
attribute determines what kind
of input they will be creating.

name
When users enter information
into a form, the server needs to
know which form control each
piece of data was entered into.
(For example, in a login form, the
server needs to know what has
been entered as the username
and what has been given as the
password.) Therefore, each form
control requires a name attribute.
The value of this attribute
identifies the form control and is
sent along with the information
they enter to the server.

Password Input

When the type attribute has
a value of password it creates
a text box that acts just like a
single-line text input, except
the characters are blocked out.
They are hidden in this way so
that if someone is looking over
the user's shoulder, they cannot
see sensitive data such as
passwords.

Lists, Tables and Forms

Bullet Point Styles

The list-style-type property
allows you to control the shape
or style of a bullet point (also
known as a marker).

Unordered Lists
For an unordered list you can use
the following values:

none
disc
circle
square

Ordered Lists
For an ordered (numbered) list
you can use the following values:

decimal
1 2 3
decimal-leading-zero
01 02 03
lower-alpha
a b c
upper-alpha
A B C
lower-roman
i. ii. iii.
upper-roman
I II III


Images for Bullets

You can specify an image to act
as a bullet point using the
list-style-image property.
The value starts with the letters
url and is followed by a pair
of parentheses. Inside the
parentheses, the path to the
image is given inside double
quotes.
This property can be used on
rules that apply to the <ul> and
*li* elements.


This property can take one of
two values:

outside
The marker sits to the left of the
block of text. (This is the default
behaviour if this property is not
used.)
inside
The marker sits inside the box of
text (which is indented).
In the example shown, the width
of the list has been limited to 150
pixels. This ensures that the text
wraps onto a new line so you can
see how the value of inside sits
the bullet inside the first line of
text.

Table Properties

You have already met several
properties that are commonly
used with tables. Here we will
put them together in a single
example using the following:

width to set the width of the
table.

padding to set the space
between the border of each table
cell and its content.

text-transform to convert the
content of the table headers to
uppercase.

letter-spacing, font-size
to add additional styling to the
content of the table headers
border-top, border-bottom
to set borders above and below
the table headers.

text-align to align the writing
to the left of some table cells and
to the right of the others.

background-color to change
the background color of the
alternating table rows.

:hover to highlight a table row
when a user's mouse goes over it

Styling Fieldsets & Legends

Fieldsets are particularly helpful
in determining the edges of a
form. In a long form they can
help group together related
information within it.
The legend is used to indicate
what information is required in
the fieldset.
Properties commonly used with
these two elements include:

width is used to control
the width of the fieldset. In
this example, the width of
the fieldset forces the form
elements to wrap onto a new line
in the correct place. (If it were
wider, the items might sit on one
line.)

color is used to control the
color of text.

background-color is used to
change the color behind these
items.

border is used to control the
appearance of the border around
the fieldset and/or legend.

border-radius is used to
soften the edges of these
elements in browsers that
support this property.

padding can be used to add
space inside these elements.

EXAMINING THE DOM IN CHROME

shows you where there
are whitespace nodes (they are
shown as # text). In the panel to
the right, you can see the value
in the nodes; whitespace nodes
have no va lue in this panel.

Firefox also has a 3D view of
the DOM, where a box is drawn
around each element, and you
can change the angle of the
page to show which parts of it
stick out more than others. The
further they protrude the further
into child elements they appear.

EVENTS

INTERACTIONS CREATE EVENTS

Events occur when users click or tap on a link, hover or swipe over an element,type on the keyboard, resize the window, or when the page they requested has loaded.

EVENTS TRIGGER CODE
When an event occurs,or fires, it can be used to trigger a particular function. Different code can be triggered when users interact with different parts of the page.

CODE RESPONDS TO USERS 
DOM can be used to update a page. The events can trigger the kinds of changes the DOM is capable of. This is how a web page reacts to users.

TRADITIONAL DOM EVENT HANDLERS

All modern browsers understand this way of creating an event handler,
but you can only attach one function to each event handler.

Below, the event handler is on
the last line (after the function
has been defined and the DOM
element node(s) selected).

When a function is called, the
parentheses that fo llow its name
tell the JavaScript interpreter to
"run this code now."

We don't want the code to
run until the event fires, so the
parentheses are omitted from
the event handler on the last line.

THE EVENT OBJECT

When an event occurs, the event object tells
you information about the event, and the
element it happened upon.

EVENT DELEGATION

Creating event listeners for a lot of elements
can slow down a page, but event flow allows
you to listen for an event on a parent element.

DIFFERENT TYPES OF EVENTS:

W3C DOM EVENTS

The DOM events specification is
managed by the W3C (who also
look after other specifications
including HTML, CSS, and XML).
Most of the events you will meet
in this chapter are part of this
DOM events specification.
Browsers implement all the
events using the same event
object that you already met.
It also provides feedback such
as which element the event
occurred on, which key a user
pressed, or where the cursor is
positioned).

HTMLS EVENTS

The HTMLS specification
(that is still being developed)
details events that browsers are
expected to support that are
specifically used with HTML.
For example, events that are
fired when a form is submitted
or form elements are changed

SOM EVENTS
Browser manufacturers also
implement some events as part
of their Browser Object Model
(or BOM). Typically these are
events not (yet) covered by
W3C specifications (although
some will be added to W3C
specifications in the future).
Several of these events dealt
with touchscreen devices:
touchstart
touchend
touchmove
orientationchange



