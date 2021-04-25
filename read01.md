## HTML5 is introducing a new set of elements that help define the structure of a page.
> Traditional HTML Layouts

For a long time, web page authors used

elements to group together related elements on the page (such as the elements that form a header, an article, footer or sidebar). Authors used class or id attributes to indicate the role of the
element in the structure of the page.
> New Html5 Layout Elements

HTML5 introduces a new set of elements that allow you to divide up the parts of a page. The names of these elements indicate the kind of content you will find in them. They are still subject to change, but that has not stopped many web page authors using them already.

- Headers & Footers
- Navigation
- Articles
- asides
- Sections
##  Extra Markup :
At this point, we have covered the main tags that fit nicely into groups and sections.

- DOCTYPEs
- Comments in HTML
- ID Attribute
- CLASS Attribute
- Block Elements
- Inline Elements
- IFrames
- Information About Your Pages
- meta

# Design web pages with CSS


> Using External CSS

#### <'link'>
The <'link'> element can be used in an HTML document to tell the browser where to find the CSS file used to style the page. It is an empty element (meaning it does not need a closing tag), and it lives inside the <'head'> element.
It should use three attributes:

* href
  - This specifies the path to the
CSS file (which is often placed in
a folder called css or styles).
- type
  - This attribute specifies the type
of document being linked to. The
value should be text/css.
- rel
  - This specifies the relationship
between the HTML page and
the file it is linked to. The value
should be stylesheet when
linking to a CSS file.

> Using Internal CSS

## style 

You can also include CSS rules within an HTML page by placing them inside a <'style'> which usually sits inside the of the page.
The <'style'>  should the type attribute to indicate that the styles are specified in
CSS. The value should be text/ css.
When building a site with more than one page, you should use
an external CSS style sheet. This:

● Allows all pages to use the same style rules (rather than
repeating them in each page).

● Keeps the content separate from how the page looks.

● Means you can change the styles used across all pages
by altering just one file (rather than each individual
page).


## Foreground Color 

> color

The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways:
1. rgb values
   - These express colors in terms of how much red, green and blue are used to make it up. For example: rgb(100,100,90)

2. hex codes
  - These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign. For example: #ee3e80

3. color names
  - There are 147 predefined color names that are recognized
by browsers. For example: DarkCyan We look at these three different ways of specifying colors on the
next double-page spread. 

> background-color

CSS treats each HTML element as if it appears in a box, and the background-color property sets the color of the background for that box.
You can specify your choice of background color in the same
three ways you can specify foreground colors: RGB values,
hex codes, and color names If you do not specify a
background color, then the background is transparent.
By default, most browser windows have a white
background, but browser users can set a background color for
their windows, so if you want to be sure that the background
is white you can use the background-color property on
the <body> element.

>  opacity 

CSS3 introduces the opacity property which allows you to
specify the opacity of an element and any of its child elements.
The value is a number between 0.0 and 1.0 (so a value of 0.5
is 50% opacity and 0.15 is 15% opacity).
The CSS3 rgba property allows you to specify a color, just like you would with an RGB value, but adds a fourth value to
indicate opacity. This value is known as an alpha value and is a number between 0.0 and 1.0 (so a value of 0.5 is 50% opacity and 0.15 is 15% opacity). 
The rgba value will only affect the element on which it is applied (not child elements).

>  hsl, hsla

The hsl color property has been introduced in CSS3 as an
alternative way to specify colors.
The value of the property starts with the letters hsl, followed by individual values inside parentheses for:

1. hue

This is expressed as an angle (between 0 and 360 degrees).


2. saturation

This is expressed as a percentage.

3. lightness

This is expressed as a percentage with 0% being white,
50% being normal, and 100% being black.
The hsla color property allows you to specify color properties using hue, saturation, and lightness as above, and adds a fourth value which represents transparency (just like the rgba property). The a stands for:

4. alpha

This is expressed as a number between 0 and 1.0.
For example, 0.5 represents 50% transparency, and 0.75
represents 75% transparency.