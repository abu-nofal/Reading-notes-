# Images 

A picture can say a thousand words, and great
images help make the difference between an
average-looking site and a really engaging one. 

> Adding Images 

< img >
To add an image into the page you need to use an < img>
element. This is an empty element (which means there is
no closing tag). 
It must carry the following two attributes:

**src**

This tells the browser where it can find the image file. 
This ill usually be a relative URL pointing to an image on your own site. 
(Here you can see that the images are in a child folder
called images — relative URLs were covered on pages 83-84).

**alt**

This provides a text description of the image which describes the image if you cannot see it.

**title**

You can also use the title attribute with the < img> element to provide additional information about the image. 
Most browsers will display the content of this attribute in a tootip when the user hovers over the image.

**height**

This specifies the height of the image in pixels.

**width**

This specifies the width of the image in pixels.

> Where to Place Images in Your Code

Where an image is placed in the code will affect how it
is displayed. 
Here are three examples of image placement
that produce different results:

1: before a paragraph

The paragraph starts on a new line after the image.

2: inside the start of a

paragraph The first row of text aligns with the bottom of the image.

3: in the middle of a

paragraph The image is placed between the words of the paragraph that it appears in.



## Foreground Color 

> color

The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways:
1. rgb values

   These express colors in terms of how much red, green and blue are used to make it up. For example: rgb(100,100,90)

2. hex codes

   These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign. For example: #ee3e80

3. color names

  There are 147 predefined color names that are recognized
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
the < body> element.

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

# text 

> font-family

The font-family property allows you to specify the
typeface that should be used for any text inside the element(s) to which a CSS rule applies.
The value of this property is the name of the typeface you want to use.
The people who are visiting your site need the typeface you have specified installed on their
computer in order for it to be displayed.
You can specify a list of fonts separated by commas so that, if the user does not have your first choice of typeface installed, the browser can try to use an
alternative font from the list.
It is also common to end with a generic font name for that type of font (which you saw on pages 269-270).

> font-size 

The font-size property enables you to specify a size for the font. 
There are several ways to specify the size of a font. The most common are:

**pixels**

Pixels are commonly used because they allow web
designers very precise control over how much space their text takes up. 
The number of pixels is followed by the letters px.
percentages The default size of text in browsers is 16px. 
So a size of 75% would be the equivalent of 12px, and 200% would be 32px.
If you create a rule to make all text inside the < body> element to be 75% of the default size (to make it 12px), and then specify another rule that indicates the content of an element inside the < body> element should be 75% size, it will be 9px (75% of the 12px font size).

**ems**

An em is equivalent to the width
of a letter m. 

> @font-face 

@font-face allows you to use
a font, even if it is not installed
on the computer of the person
browsing, by allowing you to
specify a path to a copy of the
font, which will be downloaded if
it is not on the user's machine.
Because this technique allows
a version of the font to be
downloaded to the user's
computer, it is important that the
license for the font permits it to
be used in this way.
You add the font to your style
sheet using the @font-face
rule, as shown on the right. 

> font-weight 

The font-weight property
allows you to create bold text.
There are two values that this
property commonly takes:

**normal**

This causes text to appear at a
normal weight.

**bold**

This causes text to appear bold.
In this example, you can see
that the element whose class
attribute has a value of credits
has been bolded. 

> font-style 

If you want to create italic text,
you can use the font-style
property. There are three values
this property can take:

**normal**

This causes text to appear in a
normal style (as opposed to italic
or oblique).

**italic**

This causes text to appear italic.
oblique
This causes text to appear

**oblique.**

In this example, you can see that
the credits have been italicized. 

> text-transform 

The text-transform property
is used to change the case of
text giving it one of the following
values:
**uppercase**

This causes the text to appear
uppercase.

**lowercase**

This causes the text to appear
lowercase.

**capitalize**

This causes the first letter of
each word to appear capitalized. 

>  text-decoration 

The text-decoration property
allows you to specify the
following values:

**none**

This removes any decoration
already applied to the text.

**underline**

This adds a line underneath the
text.

**overline**

This adds a line over the top of
the text.

**line-through**

This adds a line through words.

**blink**

This animates the text to make it
flash on and off (however this is
generally frowned upon, as it is
considered rather annoying). 

> letter-spacing, word-spacing 

Kerning is the term
typographers use for the space
between each letter. You can
control the space between each
letter with the letter-spacing
property.
It is particularly helpful to
increase the kerning when
your heading or sentence is
all in uppercase. If your text is
in sentence (or normal) case,
increasing or decreasing the
kerning can make it harder to
read.
You can also control the gap
between words using the
word-spacing property.
When you specify a value for
these properties, it should
be given in ems, and it will be
added on top of the default value
specified by the font.
The default gap between
words is set by the typeface
(often around 0.25em), and
it is unlikely that you would
need to change this property
regularly. If the typeface is bold
or you have increased the space
between letters, then a larger
gap between words can increase
readability. 

> text-align 

The text-align property allows
you to control the alignment of
text. The property can take one
of four values:

**left**

This indicates that the text
should be left-aligned.

**right**

This indicates that the text
should be right-aligned.

**center**

This allows you to center text.

**justify**

This indicates that every line in
a paragraph, except the last line,
should be set to take up the full
width of the containing box. 

> text-indent 

The text-indent property
allows you to indent the first
line of text within an element.
The amount you want the line
indented by can be specified in
a number of ways but is usually
given in pixels or ems. 

> text-shadow 

The text-shadow property has
become commonly used despite
lacking support in all browsers.
It is used to create a drop
shadow, which is a dark version
of the word just behind it and
slightly offset. It can also be used
to create an embossed effect by
adding a shadow that is slightly
lighter than the text.
The value of this property is
quite complicated because it can
take three lengths and a color for
the drop shadow.
The first length indicates how
far to the left or right the shadow
should fall.
The second value indicates the
distance to the top or bottom
that the shadow should fall.
The third value is optional and
specifies the amount of blur that
should be applied to the drop
shadow. 

