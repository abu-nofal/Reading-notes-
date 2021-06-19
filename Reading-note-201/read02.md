#  HTML Text, CSS Introduction, and Basic JavaScript Instructions

> Headings  

- h1  
- h2  
- h3  
- h4  
- h5  
- h6

HTML has six "levels" of headings:
< h1 > is used for main headings < h2 > is used for subheadings
If there are further sections under the subheadings then the
< h3 > element is used, and so on...

> Paragraphs  

To create a paragraph, surround the words that make up the paragraph with an opening < p> tag and closing </ p> tag.

> Bold & It alic

< b> By enclosing words in the tags < b> and </ b> we can make
characters appear bold.
The < b> element also represents a section of text that would be
presented in a visually different way (for example key words in a
paragraph) although the use of the < b> element does not imply
any additional meaning.

< i> By enclosing words in the tags < i> and </ i> we can make
characters appear italic.  
The < i> element also represents a section of text that would be
said in a different way from surrounding content — such as
technical terms, names of ships, foreign words, thoughts, or other terms that would usually be italicized.

> Line Breaks & Horizontal Rules

< br />
As you have already seen, the browser will automatically show
each new paragraph or heading on a new line. But if you wanted
to add a line break inside the middle of a paragraph you can
use the line break tag < br />.

< hr />
To create a break between themes — such as a change of
topic in a book or a new scene in a play — you can add a
horizontal rule between sections using the < hr /> tag.

> Strong & Emphasis

< strong >
The use of the < strong> element indicates that its
content has strong importance.
For example, the words contained in this element might
be said with strong emphasis.

< em>
The < em> element indicates emphasis that subtly changes
the meaning of a sentence.
By default browsers will show the contents of an < em> element
in italic.

> Quotations  

< blockquote>
The < blockquote> element is used for longer quotes that take
up an entire paragraph .  
Note how the < p> element is still used inside the < blockquote>
element.

< q>
The < q> element is used for shorter quotes that sit within
a paragraph. Browsers are supposed to put quotes around
the < q> element, however Internet Explorer does not — therefore many people avoid using the < q> element.

 > Auth or Details  

< address> 02/address.html HTML The < address> element has
quite a specific use: to contain contact details for the author of the page.
It can contain a physical address, but it does not have to. For
example, it may also contain a phone number or email address.

> Ch anges to Content  

< ins>
< del>
The < ins> element can be used to show content that has been
inserted into a document, while the < del> element can show text
that has been deleted from it .  

< s>
The < s> element indicates something that is no longer
accurate or relevant (but that should not be deleted).
Visually the content of an < s> element will usually be displayed
with a line through the center .

## Introducing CSS  

> BLOCK & INLINE ELEMENTS  

You may remember from pages 185-186 that in there is             a difference between block level and inline elements and how
how browsers display them.
Block level elements look like they start on a new line.
Examples include the < h1>- < h6>, < p> and < div> elements.
Inline elements flow within the text and do not start on a new
line.  
Examples include < b>, < i>,< img>, < em> and < span>.

> Example Styles 

- Boxes  
  - Width and height
  - Borders (color, width, and style)
  - Background color and images
  - Position in the browser window.  

- Text  
  - Typeface
  - Size  
  - Color
  - Italics, bold, uppercase,
  - lowercase, small-caps  

- Specific  
  - There are also specific ways
in which you can style certain
elements such as lists, tables,
and forms.


## Basic JavaScript Instructions 

> CREATING A BASIC JAVASCRIPT 

JavaScript is written in plain text, just like HTML and CSS,so you do not need any new tools to write a script. This example adds a greeting into an HTML page.  
The greeting changes depending on the time of day.  

- The HTML < script> element is used to load the JavaScript file into the page. It has an attribute called src, whose value is the path to the script you created.
This tells the browser to find and load the script file (just like the src attribute on an < i mg> tag).  

- try opening the
HTML file, removing the src attribute from the opening < script> tag, and adding the new code between the opening < script> tag and the closing </ script>tag.  
The s re attribute is no longer needed because the
JavaScript is in the HTML page.

> BASIC JavaScript instruction :

- COMMENTS  
  - You should write comments to explain what your code does.
They help make your code easier to read and understand.
This can help you and others who read your code.
// or /**/

- VARIABLE
  - A script will have to temporarily store the bits of information it needs to do its job. It can store this
data in variables.
- DATA TYPES  
  - JavaScript distinguishes between numbers,strings, and true or false values known as Booleans.
     -*NUMERIC DATA TYPE*
The numeric data type handles
numbers.  
     -*STRING DATA TYPE*
The strings data type consists of
letters and other characters.
    -*BOOLEAN DATA TYPE*  
Boolean data types can have one
of two values: true or false.

> RULES FOR NAMING VARIABLES

1. The name must begin with a letter, dollar sign ($),or an
underscore (_). It must not start with a number.

2. The name can contain letters, numbers, dollar sign ($), or an underscore (_). Note that you must not use a dash(-) or a period (.) in a variable name.

3. You cannot use keywords or reserved words. Keywords
are special words that tell the interpreter to do something. For example, var is a keyword used
to declare a variable. Reserved words are ones that may be used in a future version of JavaScript.
ONLINE EXTRA View a full list of keywords and
reserved words in JavaScript.

4. All variables are case sensitive, so score and Score would be different variable names, but it is bad practice to create two variables that have the same name using different cases.  

5. Use a name that describes the kind of information that the variable stores. For example, fi rstName might be used to store a person's first name, l astNarne for their last name, and age for their age.  

6. If your variable name is made up of more than one word, use a capital letter for the first letter of every word after the first word. For example, f i rstName rather
than fi rstnarne (this is referred to as camel case). You can also use an underscore between each
word (you cannot use a dash).  

> ARRAYS

An array is a special type of variable. It doesn't just store one value; it stores a list of values.
You should consider using an array whenever you are working
with a list or a set of values that are related to each other.  
Arrays are especially helpful when you do not know how
many items a list will contain because, when you create the
array, you do not need to specify how many values it will hold.
If you don't know how many items a list will contain, rather
than creating enough variables for a long list (when you might
only use a small percentage of them), using an array is
considered a better solution .  

#### CREATING AN ARRAY :

You create an array and give it a name just like you would any
other variable (using the var keyword followed by the name of
the array).
The values are assigned to the array inside a pair of square
brackets, and each value is separated by a comma. The
values in the array do not need to be the same data type, so you
can store a string, a number and a Boolean all in the same array.
This technique for creating an array is known as an array
literal. It is usually the preferred method for creating an array.
You can also write each value on a separate line:
colors= ['white',
         'black',
         'custom'];

### Operators and Loops  

A comparison operator compares its operands and returns a logical value based on whether the comparison is true. The operands can be numerical, string, logical, or object values. Strings are compared based on standard lexicographical ordering, using Unicode values. In most cases, if the two operands are not of the same type, JavaScript attempts to convert them to an appropriate type for the comparison. This behavior generally results in comparing the operands numerically. The sole exceptions to type conversion within comparisons involve the === and !== operators, which perform strict equality and inequality comparisons. These operators do not attempt to convert the operands to compatible types before checking equality. The following table describes the comparison operators in terms of this sample code:

Operator | Description  
--------- | ---------
Equal (==) |Returns true if the operands are equal
Not equal (!=)| Returns true if the operands are not equal.
Strict equal (===)| Returns true if the operands are equal and of the same type. See also Object.is and sameness in JS.  
Strict not equal (!==)|Returns true if the operands are of the same type but not equal, or are of different type.
Greater than (>)|Returns true if the left operand is greater than the right operand.
Greater than or equal (>=)|Returns true if the left operand is greater than or equal to the right operand.
Less than (<)|Returns true if the left operand is less than the right operand.
Less than or equal (<=)|Returns true if the left operand is less than or equal to the right operand.

## Loops and iteration

> for statement

A for loop repeats until a specified condition evaluates to false. The JavaScript for loop is similar to the Java and C for loop.

A for statement looks as follows:

for ([ initialExpression]; [ conditionExpression]; [ incrementExpression])
  statement

  When a for loop executes, the following occurs:
  1.The initializing expression initialExpression, if any, is executed. This expression usually initializes one or more loop counters, but the syntax allows an expression of any degree of complexity. This expression can also declare variables.
  2. The conditionExpression expression is evaluated. If the value of conditionExpression is true, the loop statements execute. If the value of condition is false, the for loop terminates. (If the condition expression is omitted entirely, the condition is assumed to be true.)
  3. The statement executes. To execute multiple statements, use a block statement ({ ... }) to group those statements.
  4. If present, the update expression incrementExpression is executed.
  5. Control returns to Step 2.

  > while statement

  A while statement executes its statements as long as a specified condition evaluates to true. A while statement looks as follows:

while (condition)
  statement

  If the condition becomes false, statement within the loop stops executing and control passes to the statement following the loop.

The condition test occurs before statement in the loop is executed. If the condition returns true, statement is executed and the condition is tested again. If the condition returns false, execution stops, and control is passed to the statement following while.

To execute multiple statements, use a block statement ({ ... }) to group those statements.

