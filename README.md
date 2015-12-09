# Test-1
test2
test3
CSS Tables
« PreviousNext Chapter »
The look of an HTML table can be greatly improved with CSS:

Company	Contact	Country
Alfreds Futterkiste	Maria Anders	Germany
Berglunds snabbköp	Christina Berglund	Sweden
Centro comercial Moctezuma	Francisco Chang	Mexico
Ernst Handel	Roland Mendel	Austria
Island Trading	Helen Bennett	UK
Königlich Essen	Philip Cramer	Germany
Laughing Bacchus Winecellars	Yoshi Tannamuri	Canada
Magazzini Alimentari Riuniti	Giovanni Rovelli	Italy
Table Borders
To specify table borders in CSS, use the border property.

The example below specifies a black border for <table>, <th>, and <td> elements:


Example
table, th, td {
   border: 1px solid black;
}
Try it yourself »
Notice that the table in the example above has double borders. This is because both the table and the <th> and <td> elements have separate borders.

Collapse Table Borders
The border-collapse property sets whether the table borders should be collapsed into a single border:


Example
table {
    border-collapse: collapse;
}

table, th, td {
    border: 1px solid black;
}
Try it yourself »
If you only want a border around the table, only specify the border property for <table>:


Example
table {
    border: 1px solid black;
}
Try it yourself »
Table Width and Height
Width and height of a table are defined by the width and height properties.

The example below sets the width of the table to 100%, and the height of the <th> elements to 50px:


Example
table {
    width: 100%;
}

th {
    height: 50px;
}
Try it yourself »
Horizontal Alignment
The text-align property sets the horizontal alignment (like left, right, or center) of the content in <th> or <td>.

By default, the content of <th> elements are center-aligned and the content of <td> elements are left-aligned.

The following example left-aligns the text in <th> elements:


Example
th {
    text-align: left;
}
Try it yourself »
Vertical Alignment
The vertical-align property sets the vertical alignment (like top, bottom, or middle) of the content in <th> or <td>.

By default, the vertical alignment of the content in a table is middle (for both <th> and <td> elements).

The following example sets the vertical text alignment to bottom for <td> elements:


Example
td {
    height: 50px;
    vertical-align: bottom;
}
Try it yourself »
Table Padding
To control the space between the border and the content in a table, use the padding property on <td> and <th> elements:


Example
th, td {
    padding: 15px;
    text-align: left;
}
Try it yourself »
Horizontal Dividers
First Name	Last Name	Savings
Peter	Griffin	$100
Lois	Griffin	$150
Joe	Swanson	$300
Add the border-bottom property to <th> and <td> for horizontal dividers:

Example
th, td {
    border-bottom: 1px solid #ddd;
}
Try it Yourself »
Hoverable Table
Use the :hover selector on <tr> to highlight table rows on mouse over:

First Name	Last Name	Savings
Peter	Griffin	$100
Lois	Griffin	$150
Joe	Swanson	$300
Example
tr:hover {background-color: #f5f5f5}
Try it Yourself »
Striped Tables
First Name	Last Name	Savings
Peter	Griffin	$100
Lois	Griffin	$150
Joe	Swanson	$300
For zebra-striped tables, use the nth-child() selector and add a background-color to all even (or odd) table rows:

Example
tr:nth-child(even) {background-color: #f2f2f2}
Try it Yourself »
Table Color
The example below specifies the background color and text color of <th> elements:

First Name	Last Name	Savings
Peter	Griffin	$100
Lois	Griffin	$150
Joe	Swanson	$300
Example
th {
    background-color: #4CAF50;
    color: white;
}
Try it Yourself »
Responsive Table
A responsive table will display a horizontal scroll bar if the screen is too small to display the full content:

First Name	Last Name	Points	Points	Points	Points	Points	Points	Points	Points	Points	Points	Points	Points
Jill	Smith	50	50	50	50	50	50	50	50	50	50	50	50
Eve	Jackson	94	94	94	94	94	94	94	94	94	94	94	94
Adam	Johnson	67	67	67	67	67	67	67	67	67	67	67	67
Add a container element (like <div>) with overflow-x:auto around the <table> element to make it responsive:

Example
<div style="overflow-x:auto;">

<table>
... table content ...
</table>

</div>
