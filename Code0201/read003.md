Ordered Lists


<ol>
The ordered list is created with
the <ol> element.
<li>
Each item in the list is placed
between an opening <li> tag
and a closing </li> tag. (The li
stands for list item.)
Browsers indent lists by default.
Sometimes you may see a type
attribute used with the <ol>
element to specify the type of
numbering (numbers, letters,
roman numerals and so on).


Unordered list 

<ul>
The unordered list is created
with the <ul> element.
<li>
Each item in the list is placed
between an opening <li> tag
and a closing </li> tag. (The li
stands for list item.)
Browsers indent lists by default.
Sometimes you may see a type
attribute used with the <ul>
element to specify the type of
bullet point (circles, squares,


Summary LISTS
There are three t XX ypes of HTML lists: ordered,
unordered, and definition.
XX Ordered lists use numbers.
XX Unordered lists use bullets.
XX Definition lists are used to define terminology.
XX Lists can be nested inside one another.'


boxes :

By default a box is sized just big
enough to hold its contents. To
set your own dimensions for a
box you can use the height and
width properties.
The most popular ways to
specify the size of a box are
to use pixels, percentages, or
ems. Traditionally, pixels have
been the most popular method
because they allow designers to
accurately control their size.
When you use percentages,
the size of the box is relative to
the size of the browser window
or, if the box is encased within
another box, it is a percentage of
the size of the containing box.
When you use ems, the size
of the box is based on the size
of text within it. Designers
have recently started to use
percentages and ems more for
measurements as they try to
create designs that are flexible
across devices which have
different-sized screens.
In the example on the right, you
can see that a containing <div>
element is used which is 300
pixels wide by 300 pixels high.
Inside of this is a paragraph
that is 75% of the width and
height of the containing element.

Border Width:
The border-width property
is used to control the width
of a border. The value of this
property can either be given
in pixels or using one of the
following values:
thin
medium
thick
(You cannot use percentages
with this property.)
You can control the individual
size of borders using four
separate properties:
border-top-width
border-right-width
border-bottom-width
border-left-width
You can also specify different
widths for the four border values
in one property, like so:
border-width: 2px 1px 1px
2px;
The values here appear in
clockwise order: top, right,
bottom, left.


border-radius:
CSS3 introduces the ability to
create rounded corners on any
box, using a property called
border-radius. The value
indicates the size of the radius
in pixels.
Older browsers that do not
support this property will show a
box with right-angled corners.
The -moz-border-radius
and -webkit-border-radius
properties are not in the CSS
specification. However, they
are used in some versions of
Chrome, Firefox, and Safari to
offer early support for this style
(and therefore can be used
to achieve this


USING A VARIABLE TO
STORE A BOOLEAN

A Boolean variable can only have
a va lue of true or fa 1 se, but this
data type is very helpful.
In the example on the right, the
values true or fa 1 se are used
in the cl ass attributes of HTML
elements. These values trigger
different CSS class rules: true
shows a check, fa 1 se shows a
cross. (You learn how the class
attribute is set in Chapter 5.)
It is rare that you would want to
write the words true or false
into the page for the user to read,
but this data type does have two
very popular uses:
First, Booleans are used when
the value can only be true/
fa 1 se. You could also think of
these values as on/off or 0/1:
true is equivalent to on or 1,
fa 1 se is equivalent to off or 0
Second, Booleans are used when
your code can take more than
one path. Remember, different
code may run in different
circumstances (as shown in the
flowcharts throughout the book).