# Lists in html 

> Ordered Lists 

< ol>
The ordered list is created with the < ol> element.
< li> Each item in the list is placed between an opening < li> tag and a closing < /li> tag. 
(The li stands for list item.)

> Unordered liste 

< ul>
The unordered list is created with the < ul> element.
< li> Each item in the list is placed between an opening < li> tag and a closing < /li> tag. 
(The li stands for list item.)

> Definition Lists

< dl>
The definition list is created with the < dl> element and usually
consists of a series of terms and their definitions.
Inside the < dl> element you will usually see pairs of  dt> and
< dd> elements.
< dt> This is used to contain the term being defined (the definition
term).
< dd> This is used to contain the definition.


## box dimention 

By default a box is sized just big enough to hold its contents.  
To set your own dimensions for a box you can use the height and
width properties.
The most popular ways to specify the size of a box are
to use pixels, percentages, or ems.  
Traditionally, pixels have been the most popular method
because they allow designers to accurately control their size.
When you use percentages, the size of the box is relative to
the size of the browser window or, if the box is encased within
another box, it is a percentage of the size of the containing box.
When you use ems, the size of the box is based on the size
of text within it. 
Designers have recently started to use percentages and ems more for
measurements as they try to create designs that are flexible
across devices which have different-sized screens.

> Limiting width 

**min-width, max-width**

Some page designs expand and shrink to fit the size of the user's
screen. In such designs, the min-width property specifies
the smallest size a box can be displayed at when the browser
window is narrow, and the max-width property indicates
the maximum width a box can stretch to when the browser
window is wide.
These are very helpful properties to ensure that the content of
pages are legible (especially on the smaller screens of handheld
devices). 
For example, you can use the max-width property to ensure that lines of text do not
appear too wide within a big browser window and you can
use the min-width property to make sure that they do not
appear too narrow.
You may find it helpful to try this example out in your browser so
that you can see what happens when you increase or decrease
the size of the browser window


> Overflowing Content 

The overflow property tells the browser what to do if the content
contained within a box is larger than the box itself. It can have
one of two values:
**hidden**
This property simply hides any extra content that does not fit in
the box.
**scroll**
This property adds a scrollbar to the box so that users can scroll
to see the missing content.
On the left, you can see two boxes whose contents expand
beyond their set dimensions. 
The first example has the overflow property with a value of hidden.
The second example has the overflow property with a value
of scroll.
The overflow property is particularly handy because some
browsers allow users to adjust the size of the text to appear as
large or as small as they want. 
If the text is set too large then the page can become an unreadable
mess. Hiding the overflow on such boxes helps prevent items
overlapping on the page.

## border 

> border-width 

The border-width property is used to control the width
of a border. 
The value of this property can either be given in pixels or using one of the
following values:
**thin**
**medium**
**thick**
(You cannot use percentages with this property.)
You can control the individual size of borders using four
separate properties:
**border-top-width**
**border-right-width**
**border-bottom-width**
**border-left-width**
You can also specify different widths for the four border values
in one property, like so:
border-width: 2px 1px 1px 2px;
The values here appear in clockwise order: top, right,
bottom, left.

> border style 

You can control the style of a border using the border-style
property. This property can take the following values:
solid a single solid line dotted a series of square dots
(if your border is 2px wide, then the dots are 2px squared with a
2px gap between each dot)
dashed a series of short lines double two solid lines (the
value of the border-width property creates the sum of the
two lines)
groove appears to be carved into the page ridge appears to stick out from
the page inset appears embedded into the page
outset looks like it is coming out of the screen
hidden / none no border is shown You can individually change the
styles of different borders using:
**border-top-style**
**border-left-style**
**border-right-style**
**border-bottom-style**

> border color 

You can specify the color of a border using either RGB values,
hex codes or CSS color names (as you saw on pages 251-252).
It is possible to individually control the colors of the borders
on different sides of a box using:
**border-top-color**
**border-right-color**
**border-bottom-color**
**border-left-color**
It is also possible to use a shorthand to control all four
border colors in the one property:
border-color: darkcyan
deeppink darkcyan
deeppink;
The values here appear in clockwise order: top, right,
bottom, left.

## padding 

The padding property allows you to specify how much space
should appear between the content of an element and its
border.
The value of this property is most often specified in pixels
(although it is also possible to use percentages or ems). 
If a percentage is used, the padding is a percentage of the browser
window (or of the containing box if it is inside another box).
Please note: If a width is specified for a box, padding is
added onto the width of the box.
As you can see, the second paragraph here is much easier
to read because there is a space between the text and the border
of the box. The box is also wider because it has padding.
You can specify different values for each side of a box using:
**padding-top**
**padding-right**
**padding-bottom**
**padding-left**
Or you can use a shorthand (where the values are in
clockwise order: top, right, bottom, left):

## margin 

The margin property controls the gap between boxes. 
Its value is commonly given in pixels, although you may also use
percentages or ems.
If one box sits on top of another, margins are collapsed , which
means the larger of the two margins will be used and the
smaller will be disregarded.
Please note: If the width of a box is specified then the margin is
added to the width of the box.
You can specify values for each side of a box using:
**margin-top**
**margin-right**
**margin-bottom**
**margin-left**
You can also use the shorthand (where the values are in
clockwise order: top, right, bottom, left):
margin: 1px 2px 3px 4px;
Sometimes you might see the following, which means that the
left and right margins should be 10 pixels and the top and bottom
margins should be 20 pixels:
margin: 10px 20px;

## box shadow 

The box-shadow property allows you to add a drop shadow
around a box. 
It works just like the text-shadow property that
you met on page 288. 
It must use at least the first of these two
values as well as a color:
Horizontal offset Negative values position the shadow to the left of the box.
Vertical offset Negative values position the shadow to the top of the box.
Blur distance If omitted, the shadow is a solid
line like a border. Sp read of shad ow If used, a positive value will
cause the shadow to expand in all directions, and a negative
value will make it contract.
The inset keyword can also be used before these values to
create an inner-shadow.

# java script (arrays)

An array is a special type of variable. It doesn't
just store one value; it stores a list of values.
You should consider using an array whenever you are working
with a list or a set of values that are related to each other.
Arrays are especially helpful when you do not know how
many items a list will contain because, when you create the
array, you do not need to specify how many values it will hold.
If you don't know how many items a list will contain, rather
than creating enough variables for a long list (when you might
only use a small percentage of them), using an array is
considered a better solution.

> CREATING AN ARRAY 

You create an array and give it a name just like you would any
other variable (using the var keyword followed by the name of
the array).
The values are assigned to the array inside a pair of square
brackets, and each value is separated by a comma. 
The values in the array do not need to be the same data type, so you
can store a string, a number and a Boolean all in the same array.
This technique for creating an array is known as an array
literal. It is usually the preferred method for creating an array.
You can also write each value on a separate line:
colors= ['white',
         'black',
         'custom']; 



> VALUES IN ARRAYS 

Values in an array are accessed as if they are in a numbered list. It is important to know that the numbering of this list starts at zero (not one). 

NUMBERING ITEMS IN AN ARRAY
Each item in an array is automatically given a number called an index. 
This can be used to access specific items in the array.  
Consider the following array which holds three colors:

var col ors;

colors= ['white ' ,
         'black ' ,
         ' custom'];

Confusingly, index values start at 0 (not 1), so the following table
shows items from the array and their corresponding index values:
**INDEX VALUE**
o   'white '
1   'black'
2   'custom'

> ACCESSING & CHANGING VALUES IN AN ARRAY 

The first lines of code on the left create an array containing a list
of three colors. (The values can be added on the same line or on separate lines as shown here.)
Having created the array, the third item on the list is changed from 'custom' to 'beige'.
To access a value from an array, after the array name you specify
the index number for that value inside square brackets.
You can change the value of an item an array by selecting it and
assigning it a new value just as you would any other variable
(using the equals sign and the new value for that item).
In the last two statements, the newly updated third item in the
array is added to the page. 

## USING SWITCH STATEMENTS

The variable called l eve 1 contains a number indicating
which level the user is on. 
This is then used as the switch value.
(The switch value could also be an expression.)
In the following code block (inside the curly braces), there
are three options for what the value of the 1eve1 variable might
be: the numbers 1, 2, or 3.
If the value of the 1eve1 variable is the number 1, the value of the
msg variable is set to 'Good luck on the first test'.
If the value is 2, it will read:
'Second of three - keep going!·
If the value is 3, the message will read: 'Final round, almost
t here! ' If no match is found, then the
value of the msg variable is set to
'Good l uck! '

## KEY LOOP CONCEPTS

Here are three points to consider when you are working with loops. Each is illustrated in examples on the following three pages. 

> KEYWORDS 

You will commonly see these two keywords used with loops:
break This keyword causes the termination of the loop and tells
the interpreter to go onto the next statement of code outside
of the loop. (You may also see it used in functions.)
continue This keyword te lls the interpreter to continue with the current
iteration, and then check the condition again. (If it is true, the code runs again.) 

>  LOOPS & ARRAYS

Loops are very helpful when dealing with arrays if you want to
run the same code for each item in the array.
For example, you might want to write the value of each item
stored in an array into the page.
You may not know how many items will be in an array when writing a script, but. 
when the code runs, it can check the total number of items in a loop. That
figure can then be used in the counter to control how many times a set of statements is run.
Once the loop has run the right number of t imes, the loop stops. 

> PERFORMANCE ISSUES 

that when a browser comes across JavaScript, it will stop doing anything else until it has processed that script.
If your loop is dealing with only a small number of items, this
will not be an issue. If, however, your loop contains a lot of items,
it can make the page slower to load. 





