# html table

> Introduction

You may want to consider using HTML tables in your website. In addition to creating HTML tables to present data in rows and columns, you can also create HTML tables to organize information on your web page.

The process of creating an HTML table is similar to the process that you used to create your web page and any elements that you may have already included in your page, such as links or frames. Coding HTML tables into your web page is fairly easy since you need only understand a few basic table codes.

> Creating a basic table

The basic structure of an HTML table consists of the following tags:

- Table tags: < TABLE> </ TABLE>
- Row tags: < TR> </ TR>
- Cell tags: < TD> </ TD>

Constructing an HTML table consists of describing the table between the beginning table tag, < TABLE>, and the ending table table tag, </ TABLE>. Between these tags, you then construct each row and each cell in the row. To do this, you would first start the row with the beginning row tag, < TR>, and then build the row by creating each cell with the beginning cell tag, < TD>, adding the data for that cell, and then closing the cell with the ending cell tag, </ TD>. When you finish all of the cells for a row, you would then close the row with the ending row tag, </ TR>.Then, for each new row, you would repeat the process of beginning the row, building each cell in the row, and closing the row.

The following table is an example of a basic table with three rows and two columns of data.

| data1 | data2 |
| ----- | ----- |
| data3 | data4 |
| data5 | data6 |

The codes that generated this table look like this:
< TABLE>
< TR>
< TD>Data 1</ TD>
< TD>Data 2</ TD>
</ TR>
< TR>
< TD>Data 3</ TD>
< TD>Data 4</ TD>
</ TR>
< TR>
< TD>Data 5</ TD>
< TD>Data 6</ TD>
</ TR>
</ TABLE>

This table contains no border, title, or headings. If you wish to add any of these elements to your table, you need to include additional HTML codes. The codes for these elements are explained in the next section.
