# Class 201 Reading Notes

* [201 Home](https://fadnesscharlie.github.io/reading-notes/201/)

## Tables

To create a Table in HTML we have certain perameters. We use the following code to start out table: `<table></table>`. Everything in our table goes in here. To create a row in our table we use `<tr></tr>` this stands for **table row**. Inside of out table row we have `<td></td>` which stands for table data. Simular to how a list is formed.

### Rows and Colums

When we want to add a column, we add `scope="col"` and `scope="row"` for rows. We add this in our `<th></th>` which stands for table header.

This looks like this:

<Table>
  <tr>
    <th></th>
    <th scope="col">PC</th>
    <th scope="col">Mac</th>
  </tr>
  <tr>
    <th scope="row">Machines in Class:</th>
    <td>50</td>
    <td>50</td>
  </tr>
  <tr>
    <th scope="row">Total Cost:</th>
    <td>$100,000</td>
    <td>$50,000</td>
  </tr>
</table>  
<br>

`<Table>`  
&nbsp;&nbsp;`<tr>`  
&nbsp;&nbsp;&nbsp;&nbsp;`<th></hd>`  
&nbsp;&nbsp;&nbsp;&nbsp;`<th scope="col">Mac</th>`  
&nbsp;&nbsp;`</tr>`  
&nbsp;&nbsp;`<tr>`  
&nbsp;&nbsp;&nbsp;&nbsp;`<th scope="row">Machines in Class:</th>`  
&nbsp;&nbsp;&nbsp;&nbsp;`<td>50</td>`  
&nbsp;&nbsp;&nbsp;&nbsp;`<td>50</td>`  
&nbsp;&nbsp;`</tr>`  
&nbsp;&nbsp;`<tr>`  
&nbsp;&nbsp;&nbsp;&nbsp;`<th scope="row">Total Cost:</hr>`  
&nbsp;&nbsp;&nbsp;&nbsp;`<td>$100,000</td>`  
&nbsp;&nbsp;&nbsp;&nbsp;`<td>$50,000</td>`  
&nbsp;&nbsp;`</tr>`  
`</table>`

<Table>
  <tr>
    <th></th>
    <th scope="col">PC</th>
    <th scope="col">Mac</th>
  </tr>
  <tr>
    <th scope="row">Machines in Class:</th>
    <td>50</td>
    <td>50</td>
    <td rowspan="2">Computers are great</td>
  </tr>
  <tr>
    <th scope="row">Total Cost:</th>
    <td>$100,000</td>
    <td>$50,000</td>
  </tr>
</table>  
<br>

In our new table, we can see that we added "Computers are great" by using `<td rowspan="2">Computers are great</td>` just below the bottom `<td>50</td>`. This works because it is taking the row below it as well because we used `rowspan="2"`.

We can do this with columns as well using `colspan="2"`.

### Long Tables

When we want to use long tables, we add in `<thead></thead>`, `<tbody></tbody>`, and `<tfoot></tfoot>`. For **table head**, **table body**, and **table footer** respectively.

Our `<thead>` is placed right above `<tr>` to hold the whole header. All of our rows will be in covered in `<tbody>`, and out footer for totals and such will be in `<tfoot>`.

## Objects

Objects are simular to an Array, but hold many different things. Some basic things is that, when updating or creating new properties we use our `object.propertyName = 'propertyValue';`. Deleting properies using the delete keyword: `delete object.propertyName;`

### New Objects

Using the new keyword in our exsisting objects, bring  a template, and add in new parametes based on what we place in them. This is very helpful so that if we want to create a template, and we want to add to it, we just: `let object = new templateObject(parameters);`

A template would like like this:

`function computer(GPU, motherboard, RAM) {`
&nbsp;&nbsp;`this.GPU = GPU;`
&nbsp;&nbsp;`this.motherboard = motherboard;`
&nbsp;&nbsp;`this.RAM = RAM;`
`}`

When we call this, we would say:

`let customBuild = new computer('RTX', 'ASUS', '32gb');`

We then just add and delete with:

`customBuild.watercooled = true`
`delete customBuild.GPU`

### Objects and Arrays

Objects and Arrays very simular. In objects we see that we always need a key/value pair. In an array its actualy the same thing. The main difference is that the we mostly see the value as the key is the index.

### Three Built-in Objects

#### Browser Object Model

This creates a mode of the browser while in a tab or window. The most used broswer object model would be window. From the window you can `window.print()` to open the broswers print dialog box. Another example is `window.screen.width;`, this shows you the width of the current screen/tab in pixels.

Some things can include `window.screenX` and `window.screenY` to get the coordinates of where your mouse is on the screen.

#### Document Object Model

The DOM creates a model of the current web page. This allows us to create, change, or remove elements and add, change, or remote text on the webpage through jsavascript.

#### Global Javascript Objects

Global Javascript Objects are multiple objects taht are different parts of the Javascript language. Some of these start with capital letters like. `String`, `Date`, and `Math`. They help objects represent basic data types, and help with real-world concepts.

Other methods that we have seen and used include: `toLowerCase()`, `split()`, and `charAt()` are some.

### GLobal Objects: Number Objects

Some methods of number objects are:

* isNaN(): Checks to see if the value is not a number
  * 42.41294
* toFixed(): Rounds the decimal to listed parameter and returns a **string**
  * Example would be: 42.413
* toPrecision(): Rounds to total number of placees and returns a **string**
  * Example would be: 42.4
* toExponential(): Returns a string represening athe number in exponential notation

### GLobal Objects: Math Objects

Some method examples would be :

`Math.round()`: Rounds the number
`Math.sqrt(n)`: Returns the square root of the parameter number
`Math.ceil()`: Rounds the number up dropped the decimal
`Math.floor()`: Rounds the number down dropped the decimal
`Math.random()`: Generates a number between 0 and 0.9, not up to 1

