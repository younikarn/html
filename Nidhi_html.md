We encounter tables everywhere, from Excel sheets to financial reports
and scientific research papers. Tables are everywhere. But have you ever
wondered how these tables are represented in websites?

In HTML, when developing a project that requires a visual representation
of data, the \<table\> tag comes to the rescue. It includes several
other tags like \<tr\>, \<td\>, \<th\>, and \<caption\>, which are
required to fill data in the table.

Let\'s dive deep into the table tag along with its child elements.:

**STRUCTURE OF TABLE:**

The table can be divided into three main sections:

**1) \<thead\>:** The \<thead\> element stands for \"table header.\" It
is used to group the header content of a table. Typically, the first row
or rows of a table, which contains header cells (\<th\>), are placed
within the \<thead\>.

This structure lets you separate the headers from the main data,
improving accessibility and styling. The use of \<thead\> is not just
for visual formatting; it helps assistive technologies like screen
readers understand the table structure better.

Example:

\<table\>

\<thead\>

\<tr\>

\<th\>Header 1\</th\>

\<th\>Header 2\</th\>

\</tr\>

\</thead\>

\<tbody\>

\<tr\>

\<td\>Data 1\</td\>

\<td\>Data 2\</td\>

\</tr\>

\</tbody\>

\</table\>

**2)\<tbody\>:** The \<tbody\> element represents the main content of
the table, typically containing the data rows (\<tr\>) with data cells
(\<td\>). While not required, using \<tbody\> can improve the structure
of your HTML code and make it more readable. It\'s advantageous in large
tables where the distinction between header and data rows becomes
essential for clarity.

Example:

\<table\>

\<thead\>

\<tr\>

\<th\>Header 1\</th\>

\<th\>Header 2\</th\>

\</tr\>

\</thead\>

\<tbody\>

\<tr\>

\<td\>Data 1\</td\>

\<td\>Data 2\</td\>

\</tr\>

\<!\-- Additional data rows \--\>

\</tbody\>

\</table\>

**3)\<tfoot\>**: The \<tfoot\> element stands for \"table footer.\" It
is used to group the footer content of a table, which might include
summary information, totals, or other data related to the table. Like
\<thead\>, using \<tfoot\> helps separate and style the footer content
appropriately.

Example:

\<table\>

\<thead\>

\<tr\>

\<th\>Header 1\</th\>

\<th\>Header 2\</th\>

\</tr\>

\</thead\>

\<tbody\>

\<tr\>

\<td\>Data 1\</td\>

\<td\>Data 2\</td\>

\</tr\>

\<!\-- Additional data rows \--\>

\</tbody\>

\<tfoot\>

\<tr\>

\<td\>Total 1\</td\>

\<td\>Total 2\</td\>

\</tr\>

\</tfoot\>

\</table\>

Now that we know about the structure of the table tag, let\'s learn more
about table cells.

TABLE ROW:

\<tr\>: It defines a single row within a table. An \<tr\> element
contains one or more table cells, which can be the table header or table
data (\<td\> or \<th\>). It is essential for structuring the rows in
your table and separating different data sets or headers.

**TYPES OF TABLE CELLS:**

In HTML, there are two main types of table cells: \<th\> and \<td\>.

**1)\<th\>:** It stands for \"table header.\" and is used for creating
cells that typically appear in the first row of a table and are meant
for headings or labels for each column. \<th\> cells are usually
displayed in bold text and are often used to provide context for the
data in the table.

Example:

\<th\>

Header Content

\</th\>

**2) \<td\>:** It stands for \"table data.\" and contains the actual
data or content for each row and column in the table. \<td\> cells
display numbers, text, or other details.

Example:

\<td\>

Data Content

\</td\>

Now, let\'s explore the operations we can perform on a table.

**OPERATIONS ON TABLE:**

**SPANNING:**

Spanning columns or rows in an HTML table allows you to merge or extend
a cell across multiple columns or rows, creating more complex and
visually appealing table layouts.

It is helpful when dealing with tables with header cells covering
multiple columns or data cells that should merge across rows to create a
more organized presentation of data.

This is achieved using the \`colspan\` and \`rowspan\` attributes within
the \`\<th\>\` or \`\<td\>\` elements.

\- \`colspan\` (Column Span): This attribute specifies how many columns
a cell should span horizontally. For example, if you set
\`colspan=\"2\"\`, the cell will cover two adjacent columns.

Example:

\<table border=\"1\"\>

\<tr\>

\<th\>Header 1\</th\>

\<th\>Header 2\</th\>

\<th\>Header 3\</th\>

\</tr\>

\<tr\>

\<td\>Data 1, Cell 1\</td\>

\<td\>Data 2, Cell 2\</td\>

\<td\>Data 3, Cell 3\</td\>

\</tr\>

\<tr\>

\<td colspan=\"2\"\>Spanning Two Columns\</td\>

\<td\>Data 4, Cell 4\</td\>

\</tr\>

\</table\>

-\`rowspan\` (Row Span): This attribute specifies how many rows a cell
should span vertically. Setting \`rowspan=\"2\"\`, for instance, causes
the cell to extend over two consecutive rows.

Example:

\<table border=\"1\"\>

\<tr\>

\<th\>Header 1\</th\>

\<th\>Header 2\</th\>

\</tr\>

\<tr\>

\<td\>Data 1, Cell 1\</td\>

\<td\>Data 2, Cell 2\</td\>

\</tr\>

\<tr\>

\<td rowspan=\"2\"\>Spanning Two Rows\</td\>

\<td\>Data 3, Cell 3\</td\>

\</tr\>

\<tr\>

\<td\>Data 4, Cell 4\</td\>

\</tr\>

\</table\>

**COLGROUP:**

The \<colgroup\> element in HTML groups and applies styling or
attributes to a set of columns within an HTML table. It is typically
placed within the \<table\> element. The primary purpose of \<colgroup\>
is to provide a way to set common properties for columns, making it more
efficient and organized than applying those properties to individual
columns or cells.

Example:

\<table\>

\<colgroup\>

\<col style=\"background-color: lightgray;\"\>

\<col style=\"background-color: lightgray;\"\>

\</colgroup\>

\<tr\>

\<td\>Column 1\</td\>

\<td\>Column 2\</td\>

\<td\>Column 3\</td\>

\</tr\>

\</table\>

**COL :**

The \<col\> element in HTML defines properties or styles for individual
columns within an HTML table. It can be used within a \<colgroup\> or
directly within a \<table\> element. The primary purpose of the \<col\>
element is to provide a way to apply column-specific formatting, layout,
or styling without the need for inline styling in each cell.

Example:

\<table\>

\<col style=\"width: 20%;\"\>

\<col style=\"width: 30%;\"\>

\<col style=\"width: 50%;\"\>

\<tr\>

\<td\>Column 1\</td\>

\<td\>Column 2\</td\>

\<td\>Column 3\</td\>

\</tr\>

\</table\>

**CELLSPACING:**

This attribute is used in the \<table\> element in HTML tables to
control the space between individual cells. It sets the space between
the boundaries of adjacent cells.

Example:

\<table cellspacing=\"10\"\>

\<tr\>

\<td\>Cell 1\</td\>

\<td\>Cell 2\</td\>

\</tr\>

\<tr\>

\<td\>Cell 3\</td\>

\<td\>Cell 4\</td\>

\</tr\>

\</table\>

**CELL PADDING:**

This attribute is used in the \<table\> element to control the space or
padding within each cell. It specifies the space between the content of
a cell and the cell\'s border.

Example:

\<table cellpadding=\"10\" border=\"1\"\>

\<tr\>

\<td\>Cell 1\</td\>

\<td\>Cell 2\</td\>

\</tr\>

\<tr\>

\<td\>Cell 3\</td\>

\<td\>Cell 4\</td\>

\</tr\>

\</table\>

And there you have it! You\'re now well-equipped to create and perform
operations on tables in HTML.

Happy coding!
