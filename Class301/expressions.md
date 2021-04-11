## My summary of reading the Responsive Web Design and Regular Expressions.


# What is Responsive Web Design and Regular Expressions:

![Responsive Designs](https://miro.medium.com/max/1838/0*DORfVSb5PrhdBet7.)

Regular expressions (regex or regexp) are extremely useful in extracting information from any text by searching for one or more matches of a specific search pattern

* One of the most interesting features is that once you’ve learned the syntax, you can actually use this tool in (almost) all programming languages ​​(JavaScript, Java, VB, C #, C / C++, Python, Perl, Ruby, Delphi, R, Tcl, and many others) with the slightest distinctions about the support of the most advanced features and syntax versions supported by the engines).

# Basic topics
1- ^ and $
^The matches any string that starts with The
end$ matches a string that ends with end
^The end$ exact string match (starts and ends with The end)
roar matches any string that has the text roar in it
? and {}
abc* matches a string that has ab followed by zero or more c
abc+ matches a string that has ab followed by one or more c
abc? matches a string that has ab followed by zero or one c
abc{2} matches a string that has ab followed by 2 c
abc{2,} matches a string that has ab followed by 2 or more c
abc{2,5} matches a string that has ab followed by 2 up to 5 c
a(bc)* matches a string that has a followed by zero or more copies of the sequence bc
a(bc){2,5} matches a string that has a followed by 2 up to 5 copies of the sequence bc

2- OR operator — | or []

a(b|c) matches a string that has a followed by b or c (and captures b or c)
a[bc] same as previous, but without capturing b or c

# Properties for the Parent (Grid container)
  *Properties for the Parent(Grid Container)
1- Display : Defines the element as a grid container and establishes a new grid formatting context for its contents.

2- Grid-template-columns , grid-template-rows : Defines the columns and rows of the grid with a space-separated list of values. The values represent the track size, and the space between them represents the grid line.

3- Grid-template-areas : Repeating the name of a grid area causes the content to span those cells.

4- Grid-template : A shorthand for setting grid-template-rows, grid-template-columns, and grid-template-areas in a single declaration.
c

5- Column-gap row-gap grid-column-gap grid-row-gap : Specifies the size of the grid lines. You can think of it like setting the width of the gutters between the columns/rows.

6- Gap grid-gap : A shorthand for row-gap and column-gap

7- Justify-items : Aligns grid items along the inline (row) axis , This value applies to all grid items inside the container.

8- Align-items : Aligns grid items along the block (column) axis , This value applies to all grid items inside the container.

9- Place-items : place-items sets both the align-items and justify-items properties in a single declaration.

10- Justify-content : This property aligns the grid along the inline (row) axis (as opposed to align-content which aligns the grid along the block (column) axis)

11- Align-content : This property aligns the grid along the block (column) axis (as opposed to justify-content which aligns the grid along the inline (row) axis).

12- Place-content : place-content sets both the align-content and justify-content properties in a single declaration.

13- Grid-auto-columns grid-auto-rows : Implicit tracks get created when there are more grid items than cells in the grid or when a grid item is placed outside of the explicit grid.

14- Grid-auto-flow : If you have grid items that you don’t explicitly place on the grid, the auto-placement algorithm kicks in to automatically place the items. This property controls how the auto-placement algorithm works.

15- Grid : A shorthand for setting all of the following properties in a single declaration: grid-template-rows, 

16- Grid-template-columns, grid-template-areas, grid-auto-rows, grid-auto-columns, and grid-auto-flow

# Properties for the Children (Grid Items)
1- Grid-column-start grid-column-end grid-row-start grid-row-end : Determines a grid item’s location within the grid by referring to specific grid lines. grid-column-start/grid-row-start is the line where the item begins, and grid-column-end grid-row-end is the line where the item ends.

2- Grid-column grid-row : Shorthand for grid-column-start + grid-column-end, and grid-row-start + grid-row-end, respectively.

3- Justify-self : Aligns a grid item inside a cell along the inline (row) axis (as opposed to align-self which aligns along the block (column) axis)

4- Align-self : Aligns a grid item inside a cell along the block (column) axis (as opposed to justify-self which aligns along the inline (row) axis). This value applies to the content inside a single grid item.

5- Place-self : place-self sets both the align-self and justify-self properties in a single declaration.

# Grid Lines

* The lines between columns are called column lines.
* The lines between rows are called row lines.

# The grid-template-columns Property
The grid-template-columns property defines the number of columns in your grid layout, and it can define the width of each column..

# The grid-template-rows Property
The grid-template-rows property defines the height of each row.


![Grid layout](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAARwAAACxCAMAAAAh3/JWAAAAtFBMVEUKCgoACQAACAAgICBkGmkABgBYGF1TF1UrDi0ECgRTF1cKCgAJD1xeGWQADlMKCgcKCiAcDB0gIBkcIGEhISwAAAAGDVwIAAAIEoMID2UKChkADU87f4ATCxMgIBAlT08UJiceFhYOGRkhISYlDShrHHFDkJEtX2BJnZ4aIIUdPT0oPT1PrK0ybG0bODg8dHUsSksoVFQmNDQeImk7ETlFE0WCIoouY2R5H39FlZcXLS5EE0jFFnKiAAAEEUlEQVR4nO3d61baQBiF4WEaQVMPVTqNBxRFAopysB7b3v99Vexv9zdrZTdO4n4vYC/yGIItaeoOtxkdpjVz3Wd07ba/MtpOa6Z/dlC9s/4rjqve+qgSmvnRP/hSvQPhJIJT1DZTI04xohzVaGYeVsxMGJ6bMxE4N6sLCk64DYSjKqZX1krMTJjPFhZyBM7FcrW0dGJwwnI+t3SicAZ35lHF4NyZZ2AUznTOwHGjYL6voi4WC8YJ6MLCfjURb6ufN5y3VUSf94IckT7K0ctpLc5e9dZHldAMDefo+Fv1jo/Smrm//F69y3t3ssvoJK0Zysruieu1sAf/SNlx2XizbY0zXxKOapy5rt9qW37HZ4Sj8l3X7RA+PNOqs8YhzAgHzAgHzAgHzAgHzAgHzAgHzAgHzAgHzAgHzAgHzAgHzAgHzAgHzNSJY35txaqBOGFQl04TcSbCeTfhgISD0gU5hYQDEg5IOCDhgIQDEg5IOCDhgIQDEg5IOCDhgIQDEg6IiOM7bcvTcMqd9tVl4WyklPecnQ4J5ylLp7LXKxk7L6wzJ/fpdJrnp4ydNn5a7e3n+f5e9Z1WfpQLByQckHBAwgEJByQckHBAwgEJByQckHBAwgG1FKcI9oNb7GrFCeZdeCSc4m6yIujUijMxb4sm4YTBM+NuyHrPHPPmVto1Z8i4j7adOMX0mXHvfp044XZ+bs2QzpzRsHFvq5X5vEHa24rxYVUvTmG+ZP2eg2aEA2aEA2aEA2aEA2aEA2aEA2aEA2aEA2aEA2aEA2aEA2aEA2YaiBPxx2nifcjpdBqBUyyGlg4P54Vx+yap8jEC58r+2oCGs8H4kVNG1nUtnDCI+NqAd+YwbhkvCa/l3+sxcZYz89RJ7JqTka7qNs5ap75rDuPTqk4cZ3+5+olxIlaEA1aEA1aEA1aEA1aEA1aEA1aEA1aEA1aEA1aEA1aEA1aEA1aEA1aEA1aEA1aEA1aEA1aEA1aEA1aEA1aEA1aEA1aEA1aEA1aEA1aEA1aEA1aEA1aEA1aEA1aEA1aEA1bqxDFvpfrEOOHc0iHi0J5NSii3ccLUvH2Th5NTHs/8svHEmHkycYrh5FcETofxo/Ks5yGTZmyc3/aNv69ncf7Rd7//h0r7bVWEqX3NeX2bf/ST1+l51qeV30nnH9+wov2eI5x3Ew5IOCDhgIQDEg5IOCDhgIQDEg5IOCDhgIQDqhWH8jDLmBqIU1AegxpT83CK2dT8W1tSzcNxYcl4unBMDcQpgs6c9ypWE/OvtEk1D4f0HwXE1ECc+hIOSDgg4YCEAxIOSDgg4YCEAxIOSDgg4YCEAxIO6O3ZpFuVe7snsPpMYvmuy8ablRuXnjGTWOPM9XJCf/wDYyaxeo5zWyppJrH+An7HCWJp3lImAAAAAElFTkSuQmCC)

# And that was it for this summary.