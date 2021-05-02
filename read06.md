# Object Literal

A JavaScript object literal is a comma-separated list of name-value pairs wrapped in curly braces. Object literals encapsulate data, enclosing it in a tidy package. This minimizes the use of global variables which can cause problems when combining code.

The following demonstrates an example object literal:

> let myObject = {

    sProp: 'some string value',
    numProp: 2,
    bProp: false  };



Object literal property values can be of any data type, including array literals, functions, and nested object literals. Here is another object literal example with these property types:

> let Swapper = {

    // an array literal
    images: ["smile.gif", "grim.gif", "frown.gif", "bomb.gif"],
    pos: { // nested object literal
        x: 40,
        y: 300
    },
    onSwap: function() { // function
        // code here
    }  };



### Object Literal Syntax

Object literals are defined using the following syntax rules:

- A colon separates property name[1] from value.
- A comma separates each name-value pair from the next.
- A comma after the last name-value pair is optional.[2]

If any of the syntax rules are broken, such as a missing comma or colon or curly brace, a JavaScript error will be triggered. Browser error messages are helpful in pointing out the general location of object literal syntax errors, but they will not necessarily be completely accurate in pointing out the nature of the error.

### Why and How We Use Object Literals

Several JavaScripts from dyn-web use object literals for setup purposes. Object literals enable us to write code that supports lots of features yet still provide a relatively straightforward process for implementers of our code. No need to invoke constructors directly or maintain the correct order of arguments passed to functions. Object literals are also useful for unobtrusive event handling; they can hold the data that would otherwise be passed in function calls from HTML event handler attributes.

There is one drawback: if you are unfamiliar with the syntax, it can be very easy to introduce errors which cause the code to stop working.

### Add a Property to an Existing Object Literal

Consider the following example object literal:

> let myObject = {

    sProp: 'some string value',
    numProp: 2,
    bProp: false  };



_You can use dot syntax to add a new property to it as follows:_

> myObject.prop2 = 'data here';

To add a new property to an object, specify the object name followed by: a dot, the name of the new property, an equals sign, and the value for the new property (enclosed in quotes if it is a string).

### Modify a Property of an Object Literal

_The following demonstrates how to access a property of an object literal:_

> alert(myObject.sProp) // display myObject.sProp value in alert
> let val = myObject.sProp; // assign myObject.sProp to variable

An expression with an object name, a dot, and a property name (myObject.sProp) will evaluate to the current value of that property. Our example first displays the value in an alert, then assigns the value to the variable val.

# Introduction to the DOM

The Document Object Model (DOM) is the data representation of the objects that comprise the structure and content of a document on the web. In this guide, we'll briefly introduce the DOM. We'll look at how the DOM represents an HTML or XML document in memory and how you use APIs to create web content and applications.

### What is the DOM?

The Document Object Model (DOM) is a programming interface for HTML and XML documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects. That way, programming languages can connect to the page.

A Web page is a document. This document can be either displayed in the browser window or as the HTML source. But it is the same document in both cases. The Document Object Model (DOM) represents that same document so it can be manipulated. The DOM is an object-oriented representation of the web page, which can be modified with a scripting language such as JavaScript.

### DOM and JavaScript

The short example above, like nearly all of the examples in this reference, is JavaScript. That is to say, it's written in JavaScript, but it uses the DOM to access the document and its elements. The DOM is not a programming language, but without it, the JavaScript language wouldn't have any model or notion of web pages, HTML documents, XML documents, and their component parts (e.g. elements). Every element in a document—the document as a whole, the head, tables within the document, table headers, text within the table cells—is part of the document object model for that document, so they can all be accessed and manipulated using the DOM and a scripting language like JavaScript.

In the beginning, JavaScript and the DOM were tightly intertwined, but eventually, they evolved into separate entities. The page content is stored in the DOM and may be accessed and manipulated via JavaScript, so that we may write this approximative equation:

> API = DOM + JavaScript

The DOM was designed to be independent of any particular programming language, making the structural representation of the document available from a single, consistent API. Though we focus exclusively on JavaScript in this reference documentation, implementations of the DOM can be built for any language
