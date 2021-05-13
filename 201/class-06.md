# Class 201 Reading Notes

* [201 Home](https://fadnesscharlie.github.io/reading-notes/201/)

## Object

An object is like an array, but with key value pairs. Instead of the `[]` we use `{}` to store the information. They **key** is the **name**, the **value** is the what you store next to the name to reference it. The value of a property can be many things, including boolean, array, string, number, or even another object. Th value of a **function** is always a **method**.

An object can not have two names, because you are using that name to reference what you want.

To call upon the object, we use the name of the object, followed by `.` then the key to access the value.

Example:

`let myCatHaru = {`
&nbsp;&nbsp;`name: 'Haru'`
&nbsp;&nbsp;`age: '1'`
&nbsp;&nbsp;`friendly: true`
&nbsp;&nbsp;`furLength: 'medium-long hair'`
&nbsp;&nbsp;`firstFunction: function() {`
&nbsp;&nbsp;&nbsp;&nbsp;`return 'Hello World'`
`}`

To pull the value name of haru. We need to write out. `myCatHaru.name`. This tells us that we want to look into the object **myCatHaru** and pull the key **name**, to then recieve **Haru**.

## DOM Document Object Model

The DOM tells the browser how it should create a model of the HTML, access, change, and update content with JS.

A DOM tree is how we get a visual understanding of what we can access and change. We start by finding the element tags, from there we can then change the attribute nodes, that are sometimes followed with text nodes. Examples would be `<h1>`, it is an attribute and has text, while `<ul>`, is just an element as the attribute is in `<li>`.

### Working with the DOM Tree

In working with the DOM tree, there are two steps:

Step one: Access the Elements

Examples of this would be, `getElementById()`, `getElementsByClassName()`, `parentNode`, `querySelector()`, `getElementByTagName()`, `querySelectorAll()`, `previousSibling/nextSibling`, and `firstChild/lastChild` are some examples.

Step two: Work with Those Elements

Examples of this would be: `let idUpdate = document.getElementById('idNameHere')` then we can simply idUpdate. Write whatever you would like here, whether you are trying to add content, or change. This looks through the HTML document and grabs an element with `id=idNameHere`.

As with changing, you can create, append, and remove things as well.

When talking about storing an element, we store those elements in variables to make calling them later easier for us. `let exampleOne = getElementById('storeThis');`

### Accessing Elements

When we want to access elements, a good understanding is if the elements come individually or if they come in a Nodelist. We know that the `id=""` is unique and will only rturn one element with `getElementById()`, while `class=""` has many elements and will come in a Nodelist most of the time `getElementsByClassName()`, depending on how many classes there are.

Breaking down the code. `document.getElementById('idNameHere')`:

`document` is the object.

`.` is the member operator.

`getElementById` is the method.

`'idNamehere'` is the parameter.

### Nodelist

When calling a Nodelist, the elements that are grabbed are stored using an index number, simular to an array. In which position it will be at is when it was grabbed. As it reads through the HTML, as it finds the first, it will be at index 0, and so on.

### Selecting from a Nodelist

In a nodelist, there are two ways access elements in a Nodelist, one is ` item()` method, and the other is Array Syntax. We first want to make sure there are elements in this Nodelist. You will always want to run an if statement declaring that if there are 1 or more elements in the Nodelist, then run this code, as you do not want to run the code if there are no elements in the Nodelist.

Method: `item()`

`let ifElements = document.getElementsByClassName('classNameHere')`
`if (ifElements.length >= 1) {`
&nbsp;&nbsp;`let foundElement = ifElements.item(0);`
`}`

Array Syntax:

`let ifElements = document.getElementsByClassName('classNameHere')`
`if (ifElements.length >= 1) {`
&nbsp;&nbsp;`let foundElement = ifElements[0];`
`}`

### Traversindf the DOM

With travering, we can use `parentNode`, `previousSibling/nextSibling`, and `firstChild/lastChild` to cycle through.

### White Space

Having whitespace will be a challenging, jquery helps with this, but there will most likely be *white space* in between your elements.

### Using the DOM

While using the DOM, there are many things you can do, some of those things include, creating HTML elements, adding text into those elements. Updating and removing elements are very handy, think of if the user clicked something, you can have the class changed which then runs a new set of CSS rules to display to the user.

Things to note, you can classify something using methods, here are some examples: `getAttribute()`, `hasAttribute()`, `setAttribute()`, or `removeAttribute()`.

Being able to control the DOM, makes it very simple to change things when something runs, being able to set certain rules, updating, creating, or even removing elements, text, or even markup is very powerful!
