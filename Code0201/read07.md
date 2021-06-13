Basic Table Structure

*table*
The table element is used
to create a table. The contents
of the table are written out row
by row.
<tr>
You indicate the start of each
row using the opening <tr> tag.
(The tr stands for table row.)
It is followed by one or more
<td> elements (one for each cell
in that row).
At the end of the row you use a
closing </tr> tag.
<td>
Each cell of a table is
represented using a <td>
element. (The td stands for
table data.)
At the end of each cell you use a
closing </td> tag.

Table Headings

*th*
The <th> element is used just
like the <td> element but its
purpose is to represent the
heading for either a column or
a row. (The th stands for table
heading.)
Even if a cell has no content,
you should still use a <td> or
<th> element to represent
the presence of an empty cell
otherwise the table will not
render correctly. (The first cell
in the first row of this example
shows an empty cell.)
Using <th> elements for
headings helps people who
use screen readers, improves
the ability for search engines
to index your pages, and also
enables you to control the
appearance of tables better
when you start to use CSS.
You can use the scope attribute
on the <th> element to indicate
whether it is a heading for a
column or a row. It can take the
values: row to indicate a heading
for a row or col to indicate a
heading for a column.
Browsers usually display the
content of a <th> element in
bold and in the middle of the cell.


Spanning ColumnS

Sometimes you may need the
entries in a table to stretch
across more than one column.
The colspan attribute can be
used on a <th> or <td> element
and indicates how many columns
that cell should run across.
In the example on the right
you can see a timetable with
five columns; the first column
contains the heading for that
row (the day), the remaining four
represent one hour time slots.
If you look at the table cell that
contains the words 'Geography'
you will see that the value of the
colspan attribute is 2, which
indicates that the cell should run
across two columns. In the third
row, 'Gym' runs across three
columns.
You can see that the second
and third rows have fewer
<td> elements than there are
columns. This is because, when
a cell extends across more than
one column, the <td> or <th>
cells that would have been in the
place of the wider cells are not
included in the code.

spanning rows


You may also need entries in
a table to stretch down across
more than one row.
The rowspan attribute can be
used on a <th> or <td> element
to indicate how many rows a cell
should span down the table.
In the example on the left you
can see that ABC is showing a
movie from 6pm - 8pm, whereas
the BBC and CNN channels are
both showing two programs
during this time period (each of
which lasts one hour).
If you look at the last <tr>
element, it only contains three
elements even though there are
four columns in the result below.
This is because the movie in the
<tr> element above it uses the
rowspan attribute to stretch
down and take over the cell
below.

Long Tables

There are three elements that
help distinguish between the
main content of the table and
the first and last rows (which can
contain different content).
These elements help people
who use screen readers and also
allow you to style these sections
in a different manner than the
rest of the table (as you will see
when you learn about CSS).
*thead*
The headings of the table should
sit inside the <thead> element.
*tbody*
The body should sit inside the
tbody element.
*tfoot*
The footer belongs inside the
*tfoot* element.
By default, browsers rarely treat
the content of these elements
any differently than other
elements however designers
often use CSS styles to change
their appearance.


Width & Spacing

There are some outdated
attributes which you should not
use on new websites. You may,
however, come across some
of them when looking at older
code, so I will mention them
here. All of these attributes have
been replaced by the use of CSS.
The width attribute was used
on the opening <table> tag to
indicate how wide that table
should be and on some opening
<th> and <td> tags to specify
the width of individual cells.
The value of this attribute is
the width of the table or cell in
pixels.
The columns in a table need to
form a straight line, so you often
only see the width attribute on
the first row (and all subsequent
rows would use that setting).
The opening <table> tag could
also use the cellpadding
attribute to add space inside
each cell of the table, and the
cellspacing attribute to create
space between each cell of
the table. The values for these
attributes were given in pixels.

ADDING AND REMOVING
PROPERTIES

Once you have created an object
(using literal or constructor
notation), you can add new
properties to it.
You do this using the dot
notation that you saw for adding
properties to objects on pl03.
In this example, you can see that
an instance of the hotel object
is created using an object literal.
Immediately after t his, the
hotel object is given two
extra properties that show the
facilities (whether or not it has
a gym and/or a pool). These
properties are given values that
are Booleans (true or false).
Having added these properties
to the object, you can access
them just like any of the objects
other properties. Here, they
update the value of the cl ass
attribute on their respective
elements to show either a check
mark or a cross mark.
To delete a property, you use
the keyword delete, and then
use dot notation to identify the
property or method you want to
remove from the object.
In this case, the booked property
is removed from the object.

GLOBAL OBJECTS:
STRING OBJECT

Whenever you have a value that is a string, you can use the properties
and methods of the String object on that valu e. This example stores the phrase "Home sweet home " in a variable.

These properties and methods
are often used to work with text
stored in variables or objects.
On the right-hand page, note
how the variable name (saying)
is followed by a dot, then the
property or method that is being
demonstrated (like the name of
an object is fo llowed by a dot
and its properties or methods).
This is why the String object is
known as bot h a global object,
because it works anywhere
within your script, and a wrapper
object because it acts like a
wrapper around any value that
is a string - you can use this
object's properties and methods
on any value that is a string.
The length property counts
the number of "code units" in a
string. In the majority of cases,
one character uses one code
unit, and most programmers use
it like this. But some of the ra rely
used characters take up two
code units.

GLOBAL OBJECTS: NUMBER OBJECT

Whenever you have a value that is a number,
you can use the methods and properties of the
Number object on it.

