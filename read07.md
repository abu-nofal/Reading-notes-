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


# Object Constructors

> function Person(first, last, age, eye) {
  this.firstName = first;
  this.lastName = last;
  this.age = age;
  this.eyeColor = eye;
}

Object Types (Blueprints) (Classes)
The examples from the previous chapters are limited. They only create single objects.

Sometimes we need a "blueprint" for creating many objects of the same "type".

The way to create an "object type", is to use an object constructor function.

In the example above, function Person() is an object constructor function.

Objects of the same type are created by calling the constructor function with the new keyword:
> let myFather = new Person("John", "Doe", 50, "blue");

>let myMother = new Person("Sally", "Rally", 48, "green");

The **this** Keyword
In JavaScript, the thing called **this** is the object that "owns" the code.

The value of **this**, when used in an object, is the object itself.

In a constructor function **this** does not have a value. It is a substitute for the new object. The value of **this** will become the new object when a new object is created.

### Adding a Property to an Object
Adding a new property to an existing object is easy:
> myFather.nationality = "English";

### Adding a Method to an Object
Adding a new method to an existing object is easy:
> myFather.name = function () {
  return this.firstName + " " + this.lastName;
};

## Adding a Property to a Constructor

You cannot add a new property to an object constructor the To add a new property to a constructor, you must add it to the constructor function:

> function Person(first, last, age, eyecolor) {
  this.firstName = first;
  this.lastName = last;
  this.age = age;
  this.eyeColor = eyecolor;
  this.nationality = "English";
}

## Adding a Method to a Constructor
Your constructor function can also define methods: 

> function Person(first, last, age, eyecolor) {
  this.firstName = first;
  this.lastName = last;
  this.age = age;
  this.eyeColor = eyecolor;
  this.name = function() {return this.firstName + " " + this.lastName;};
}
You cannot add a new method to an object constructor the same way you add a new method to an existing object.

Adding methods to an object constructor must be done inside the constructor function:
> function Person(firstName, lastName, age, eyeColor) {
  this.firstName = firstName; 
  this.lastName = lastName;
  this.age = age;
  this.eyeColor = eyeColor;
  this.changeName = function (name) {
    this.lastName = name;
  };
}


