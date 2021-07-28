# HTML Lists, CSS Boxes, JS Control Flow

- [Home](https://fadnesscharlie.github.io/reading-notes/201/) 

## Lists

### Numbered/Ordered List

We apply ordered list with the tags `<ol></ol>`, the ol, meaning **Ordered List**. Inside of our list we have `<li></li>`, which means, **List Item**.

An Example of an Ordered list would be:  
<ol>
<li>Our first item in our ordered list</li>
<li>Our Second item in our ordered list</li>
<li>And our third item in our ordered list</li>
</ol>

The coding behind it looks like:  

`<ol>`  
&nbsp;&nbsp;&nbsp;&nbsp;`<li>Our first item in our ordered list</li>`  
&nbsp;&nbsp;&nbsp;&nbsp;`<li>Our Second item in our ordered list</li>`  
&nbsp;&nbsp;&nbsp;&nbsp;`<li>And our third item in our ordered list</li>`  
`</ol>`

We create our tags for ordered list, then we include our list item to show what you want in each list item, and where does it end.

### Bullet/Unordered Lists

Unordered list are very simular to the above. The one thing that changes is the `<ol></ol>`, we change that to `<ul></ul>` which means **Unordered List**. To create:  
<ul>
<li>Our first item in our unordered list</li>
<li>Our Second item in our unordered list</li>
<li>And our third item in our unordered list</li>
</ul>

The coding behind it looks like:  

`<ul>`  
&nbsp;&nbsp;&nbsp;&nbsp;`<li>Our first item in our unordered list</li>`  
&nbsp;&nbsp;&nbsp;&nbsp;`<li>Our Second item in our unordered list</li>`  
`<li>And our third item in our unordered list</li>`  
`</ul>`

Which makes it very simple to remember and implement!

### Definition Lists

Defintion lists are a little different then the ones we saw before, they are more complex then the simple list.

Here we have three types of tags, and not just two.   
We use `<dl></dl>` which stands for **Definition List**, `<dt></dt>` which stands for **Definition Term**, and lastly `<dd></dd>` which stands for **Definition**.

<dl>
<dt>Cat</dt>
<dd>A small domesticated carnivorous mammal with soft fur, a short snout, and retractable claws. It is widely kept as a pet or for catching mice, and many breeds have been developed</dd>
<dt>Ailurophile</dt>
<dd>A cat lover</dd>
<dt>Dog</dt>
<dd>A domesticated carnivorous mammal that typically has a long snout, an acute sense of smell, nonretractable claws, and a barking, howling, or whining voice</dd>
<dt>Caninophile</dt>
<dd>Someone who loves dogs</dd>
</dl>

We see that our definitons are indented for us for better readability by the tag itself. This makes it easy to know which is the word, and which is the definition.

The Code for this would be: 

`<dl>`  
`<dt>Cat</dt>`  
`<dd>A small domesticated carnivorous mammal with soft fur, a short snout, and retractable claws. It is widely kept as a pet or for catching mice, and many breeds have been developed</dd>`  

`<dt>Ailurophile</dt>`  
`<dd>A cat lover</dd>`  
`<dt>Dog</dt>`  

`<dd>A domesticated carnivorous mammal that typically has a long snout, an acute sense of smell, nonretractable claws, and a barking, howling, or whining voice</dd>`

`<dt>Caninophile</dt>`  
`<dd>Someone who loves dogs</dd>`  
`</dl>`  

We can see that we do not need have everything in between each corresponding tags. Its a little difficult to read it all like this, but thats why the computer indents it for the user.

### Nested Lists

Nested lists are lists that are tabbed into more smaller list.

<ul>
<li>Our first item in our unordered list</li>
<li>Our Second item in our unordered list
<ul>
<li>Here is our nested list.</li>
<li>We can go on and on in our nested list as well</li>
</ul>
</li>
<li>And our third item in our unordered list</li>
</ul>

We can do this with Ordered List as well.
<ol>
<li>Our first item in our unordered list</li>
<li>Our Second item in our unordered list
<ol>
<li>Here is our nested list.</li>
<li>We can go on and on in our nested list as well</li>
</ol>
</li>
<li>And our third item in our unordered list</li>
</ol>

The code behind this looks like:

`<ul>`  
`<li>Our first item in our unordered list</li>`  
`<li>Our Second item in our unordered list`  
`<ul>`  
`<li>Here is our nested list.</li>`  
`<li>We can go on and on in our nested list as well</li>`  
`</ul>`  
`</li>`  
`<li>And our third item in our unordered list</li>`  
`</ul>`  

Notice that the order is a little different, we are adding a new `<ul></ul>` inside of one of our `<li></li>`, specifically our **Second item**. We even move the end of `</li>` to just before we want to continue so we set the boundary in which we want our nested list to be.

## Boxes

### Limited Height with Min and Max

From what you remember when we used say `<p></p>` tags, we can modify those. Because each of those tags create their own box, think of the wire frame we used to create our HTML pages.

<div style =" height: 300px; width: 400px; background-color: red;">
<p style ="height: 70%; width: 70%; background-color: blue;">
Let's create some text in here to create our box shall we!
</p>
</div>
 Below is the code we used for our box.

`<div>`  
&nbsp;&nbsp;&nbsp;&nbsp;`<p>`  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`Let's create some text in here to create our box shall we!`  
&nbsp;&nbsp;&nbsp;&nbsp;`</p>`  
`</div>`

In our box above, we added a `<div></div>` tag and inside a `<p></p>` tag. We added some CSS to it so you can see the what setting a width and height can be.

`div {`  
&nbsp;&nbsp;&nbsp;&nbsp;`height: 300px;`  
&nbsp;&nbsp;&nbsp;&nbsp;`width: 400px;`  
&nbsp;&nbsp;&nbsp;&nbsp;`background-color: red;`  
`}`

`p {`  
&nbsp;&nbsp;&nbsp;&nbsp;`height: 70%;`  
&nbsp;&nbsp;&nbsp;&nbsp;`width: 70%;`  
&nbsp;&nbsp;&nbsp;&nbsp;`background-color: blue;`  
`}`

As you can see the height and width set for both boxes, one set with px or pixels, and the other set with percentages. There is a third way of setting those as well with `em`.

### Percentages

Percentages have the advanage of looks, you can set something within something without having to know how many pixels, the downfall of this is that it is based on the users window. Whether it be from their computer, tablet, or even their phone. Sometimes it can compress your text or information inside.

### Pixels

Pixels have their advantage because now you be exact in how you want to see it across multiple platforms and stay the same.

### Ems

Ems and Percentages have been more commonly used. Ems base the size on the text inside the box which is very helpful in cases where you dont want words to leak or be compressed when seeing the same page over different screen types and platforms.

### Min-Maxing

With wanting to min and max the width for certain devices, below is an example of that. This is nice for people who may be viewing it on an extra large screen, or a very high pixel screen. An example would be, we wouldnt want this to take over the whole screen if someone had a 70inch 4k TV they were viewing it on.

When limiting the height and width, you want to make sure to ame sure all of your content is inside the box, for if you have to much content and not enough space, the text will start to spill out and compress it, and it will not look good to anyone anymore. 

`p {`  
&nbsp;&nbsp;&nbsp;&nbsp;`min-height: 70%;`  
&nbsp;&nbsp;&nbsp;&nbsp;`max-height: 70%;`   
`}`

### Overflow

When dealing with oveflow, we have two options, we can hide the content, it willc ut off the extra text, which creates space, or adds a scroll feature which makes the content fit inside the box while scrolling through that box.

`p {`  
&nbsp;&nbsp;&nbsp;&nbsp;`overflow: hidden`  
&nbsp;&nbsp;&nbsp;&nbsp;`overflow: scroll`  
`}`

## Border, Margin, and Padding

We can adjust the size, and distance of each side while using borders, margins, or paddings. We can set certain number of pixels "margin: 25px;", or even percentage "padding: 25%;". In the image below, we are using pixels.

<div style ="
height: 100px;
width: 100px;
background-color: cadetblue;
border-width: 5px 10px 15px 20px;
border-style: solid;
border-color: brown;
padding: 25px;
margin: 25px;
float: left;
">
This Box shows our Margin, Border, and Padding!
</div>

### Margin

For our Margin, our distance from our text and box is our margin. We can't see it, buts still there and gives us space around our object/box.

### Border

Our border is the color red for reference. We can clearly see this as it wraps around our words. It connects between the margin and padding.

### Padding

Last but not least, our padding. Here can see the distance from the border to our words. This is the padding.

## White Space and Vertical Margin

Adding in the amount of margins and padding can help a lot by putting distance inbetween two different subjects to create spacing and white space. If not, you might have two boxes that are literally touching each other and can confuse the user thinking those two boxes are related when they might be different.

## Border Styles

There a lot of different types of border styles. Using the syntax of "border-style: solid;" You can change the solid to "dotted", "dashed", "double", "groove", "ridge", "inset", and "outset". Try it out to see all possible ways you can style your border!

## Border Color

Lets take the reference from above. With the size of the border. You can see that the border has a few different sizes, as you can size each one differently! With colors, you can do that same!

<div style ="
height: 100px;
width: 100px;
background-color: cadetblue;
border-width: 5px 10px 15px 20px;
border-style: solid;
border-color: red blue green yellow;
padding: 25px;
margin: 25px;
float: left;
"> Our colors box</div>

The way we achieve this is by specifying the border color, then giving it four different colors to take in.  
`<div>`  
&nbsp;&nbsp;`border-color: red yellow green blue`  
`</div>`  

Notice how it starts from top, then left, then bottom, then right in that order. That is how CSS operates by itself unless we specify where we want

## Centering Content

When you want to center the content. You can easily center all the content on the page with a simple `text-align: center;` if either your main body, or any boxes. You can even add a `text-align:left;`, `text-align:left;`, up, or even down.

When aligning text inside of a box, the text align is inherited by the child elements. You will need to set the text inside of the box incase you do not want that text to be aligned the same as the whole box.

## Changing Inline/Block and Hiding Boxes

### Chaning Inline/Block Elements

<!-- Following Example took from HTML/CSS Book Jon Ducket Page 317/318 -->
</br>

#### Example 1

<ul style ="border: solid black;">
&nbsp;&nbsp;<li style ="display: inline; margin-right: 10px;">Home</li>
&nbsp;&nbsp;<li style ="display: inline; margin-right: 10px;">Products</li>
&nbsp;&nbsp;<li style ="display: inline; display: none;margin-right: 10px;" class="coming-soon">Services</li>
&nbsp;&nbsp;<li style ="display: inline; margin-right: 10px;">About</li>
&nbsp;&nbsp;<li style ="display: inline;">Contact</li>
</ul>

</br>

</br>

#### Example 2

<ul style ="border: solid black;">
&nbsp;&nbsp;<li style ="display: inline; margin-right: 10px;">Home</li>
&nbsp;&nbsp;<li style ="display: inline; margin-right: 10px;">Products</li>
&nbsp;&nbsp;<li style ="display: inline; visibility: hidden;margin-right: 10px;">Services</li>
&nbsp;&nbsp;<li style ="display: inline; margin-right: 10px;">About</li>
&nbsp;&nbsp;<li style ="display: inline;">Contact</li>
</ul>

</br>

#### HTML

`<ul>`  
&nbsp;&nbsp;`<li>Home</li>`  
&nbsp;&nbsp;`<li>Products</li>`  
&nbsp;&nbsp;`<li class="coming-soon">Services</li>`  
&nbsp;&nbsp;`<li>About</li>`  
&nbsp;&nbsp;`<li>Contact</li>`  
`</ul>`

#### CSS

`li {`  
&nbsp;&nbsp;`display: inline;`  
&nbsp;&nbsp;`margin-right: 10px;`  
`}`  

`li.coming-soon {`  
&nbsp;&nbsp;`display: none;`  
`}`

`li.coming-soon {`  
&nbsp;&nbsp;`visibility: hidden;`  
`}`

As you can see above, we can change our simple list, to display them together inline with one another, and giving them some simple spacing with a little extra margins.

Notice that the our Example 1, the middle "Services" does not show because we added a class to specify that specific one and took it out with `display: none;`.

In our Example two, we have it hidden with `visibility: hidden`. This not only removes it, but it keeps it place holder there and keep a blank space there.

But do keep note that just because you have it hidden, if someone reads the souce code, they can see that it is hidden from the page and can still go to it.

## Box Shadows, Rounded Corners, and Elliptical Shapes

### Box Shadows

<p style=" float: left; margin-left: 30px; width: 100px; height: 100px; background-color: blue; box-shadow: -5px -5px #777777">Example One</p>

<p style=" float: left; margin-left: 30px; width: 100px; height: 100px; background-color: blue; box-shadow: 5px 5px 5px #777777">Example Two</p>

<p style=" float: left; margin-left: 30px; width: 100px; height: 100px; background-color: blue; box-shadow: 5px 5px 5px 5px #777777">Example Three</p>

<p style=" float: left; margin-left: 30px; width: 100px; height: 100px; background-color: blue; box-shadow: 0 0 10px #777777">Example Four</p>

<p style=" float: left; margin-left: 30px; width: 100px; height: 100px; background-color: blue; box-shadow: inset 0 0 10px #777777">Example Five</p>

<br><br><br><br><br><br>

Above we have 5 examples. In each example is how you can add box shadows to the background of images to add perspective of the image. Below is how we add this to our image.

Using `<p class="Example #">Example #</p>` for the boxes and adding in some color, widthm height for example purposes will be our boxes. They gray behind or inside is what we are adding or changing.

`p.exampleOne {`  
&nbsp;&nbsp;`box-shadow: -5px -5px #777777`  
`}`

`p.exampleTwo {`  
&nbsp;&nbsp;`box-shadow: 5px 5px 5px #777777`  
`}`

`p.exampleThree {`  
&nbsp;&nbsp;`box-shadow: box-shadow: 5px 5px 5px 5px #777777`  
`}`

`p.exampleFour {`  
&nbsp;&nbsp;`box-shadow: 0 0 10px #777777`  
`}`

`p.exampleFive {`  
&nbsp;&nbsp;`box-shadow: inset 0 0 10px #777777`  
`}`

While using different pixels, we can change the side and how it appears. Note that you can change the color of the box shadow as well. It does not have to be limited to just this color in the example.

### Rounded Corners

<p style="border: 5px solid red;
  padding 20px;
  width 250px;
  border-radius: 10px;">In here we are going to show how you can add rounded corners to either a text or an image. With the following code:</p> 

`p {`  
&nbsp;&nbsp;`border: 5px solid red;`  
&nbsp;&nbsp;`padding 20px;`  
&nbsp;&nbsp;`width 250px;`  
&nbsp;&nbsp;`border-radius: 10px;`  
`}`

### Elliptical Shapes

Elliptical shapes are differnet then the usual shapes, what we can do a lot differnt, as instead of just adding a corner to the image or text, we are going modify the corners in any way or shape that we want.

<p style="border-top-left-radius: 80px 50px;border: 5px solid blue; padding: 20px;">
<b>Example One</b><br>
 In this example what we have is, we are modifying just one corner, notice that is not a perfect corner, but instead we make one side more curve or angle more then the other. Notice how we specify the top-left only, as if we took that out, it would instead effect every corner</p>

#### Code for Example One looks like:

`p.ExampleOne {`  
&nbsp;&nbsp;`border-top-left-radius: 80px 50px;`  
`}`


<p style="border-radius: 1em 5em 1em 5em / 3em 1em 3em 1em; border: 5px solid blue; padding: 20px;">
<b>Example Two</b><br>
In this example we modify very carefully using em. We add four, targeting every corner which means we do not need to clarify which corner as it has its own corners. We first add the horizonal values, the add the veritcal values and sperate it with an "/".</p>

#### Code for Example two looks like:

`p.ExampleOne {`  
&nbsp;&nbsp;`border-radius: 1em 5em 1em 5em / 3em 1em 3em 1em;`  
`}`

<p style="border-radius: 500px;border: 5px solid blue; padding: 35px; width: 250px">
<b>Example Three</b><br>
In our last example here, we modify each corner to the same. We state one pixel for each corner so it can be the same for each side. Since we have text and not an image, creating a perfect circle is more difficult depending on the width of the page vs just cropping the image.</p>

#### Code for Example Three looks like:

`p.ExampleOne {`  
&nbsp;&nbsp;`border-radius: 500px;`  
`}`

## Moving Into JavaScript:

## Arrays

Stores not just one variable, but multiple variables. This can consist of strings, booleans, and numbers in any order.

Use an array when working with a list or a set of values that are related to each other, an example of this would be a shopping cart, it consist of many values that are related to each other. Its nice when you dont need to know how many values you can hold.

Example:  
`var colors;`  
`colors = ['red', 'blue', 'custom'];`  

A new method is using the `Array();` keyword  

`var colors = new Array('red',`  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`'blue',`  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`'custom');`  

When calling upon an array, you call by their number position. But note that numbers start at 0. In the example above, red[0], blue[1], custom[2].

Example:  
`var gettingItem;`
`gettingItem = colors[1];`

Which would get back `blue`.

Using the length keyword we can retrieve how many values are in our array.

`var numbColor;`  
`numbColors = colors.length;`

<!-- Taken from "JavaScript & Jquery by Jon Duckett" Page 73 -->

### Accessing & Changing Values in an Array

Below we will assign a new color in the array by replacing it. We will change `'custom'` to `'beige'`.

Create the array  
`var colors = ['white', 'black', 'custom'];`

Update the third item in the array  
`colors[2] = 'beige';`

Get the element with an id of the colors  
`var el = document.getElementById('colors');`

Replace with third item from the array  
`el.textContent = colors[2];`

<!-- end -->

## If, else if, and else Statements

In if statements, we check to see if something is true, when it is true, it runs the following code in the code block under the if statement.

An Example of this would be:  

`if carSpeed > 65 {`  
&nbsp;&nbsp;&nbsp;&nbsp;`slowDown();`  
`} else if carSpeed < 55 {`  
&nbsp;&nbsp;&nbsp;&nbsp;`speedUp();`  
`} else {`
&nbsp;&nbsp;&nbsp;&nbsp;`staySameSpeed();`
`}`

In this case, we also see an else if, and else statements as well. We can see that our if statement asks if our carSpeed variable is more then 65, if it would be, we would slowDown. If our car speed was less then 65, it would move to the next statement, which would be else if our carSpeed was slower then 55, we would speedUp. And if our carSpeed was in the middle of both 55 and 65, we would stay the same speed.

## Switch Statements

In switch statements. They are very simular to if statements. As we go through, if you need an example, if think of multiple if statements running, if true, then it runs that. That is almost the same thing, the only reason to use this, looks a little better, takes a value, and runs faster then multiple if statements.

In our example. Let us run a test to see the spicy level of food the user or document may want/offer.

In our code block, it will look something like this:

`let verifySpicy;`  
`let spiceLevel = 1;`

`switch (spiceLevel) {`  
&nbsp;&nbsp;`case 1:`  
&nbsp;&nbsp;&nbsp;&nbsp;`verifySpice = 'This is our lowest spice level, just above adding no spice level.'`  
&nbsp;&nbsp;&nbsp;&nbsp;`break;`

&nbsp;&nbsp;`case 2:`  
&nbsp;&nbsp;&nbsp;&nbsp;`verifySpice = 'This is our low-medium spice level, you will taste some spice level, but nothing to heavy.'`  

&nbsp;&nbsp;`case 3:`  
&nbsp;&nbsp;&nbsp;&nbsp;`verifySpice = 'This is our medium spice level, most people choose this.'`  
&nbsp;&nbsp;&nbsp;&nbsp;`break;`

&nbsp;&nbsp;`case 4:`  
&nbsp;&nbsp;&nbsp;&nbsp;`verifySpice = 'This is our medium-high spice level, you will feel some burn here.'`  
&nbsp;&nbsp;&nbsp;&nbsp;`break;`

&nbsp;&nbsp;`case 5:`  
&nbsp;&nbsp;&nbsp;&nbsp;`verifySpice = 'This is our highest spice level, enter at your own risk here.'`  
&nbsp;&nbsp;&nbsp;&nbsp;`break;`  
`}`

Above we can see our switch statement. Know that our variable, or what we are comparing at is our numbers which would be 1, 2, 3, 4, or 5. We could name each of our numbers as low, medium, or high as other examples. Our variable that takes in the variable is spiceLevel.

## Type Coercion and Weak Typing

Type coercion is JavaScript behind the scenes trying to make sense of things. If we have a number lets say 20, instead of JS trying to make an error, it will evaluate to either number `20`, or string `'20'`. This makes it so the code will run, but can make it difficult later on. That is why JS uses strict operators. This is to prevent the code determining it differently or guessing which value you are trying to display. As a strict `===` will have to be exact to either the string or number while a basic `==` will evalute both cases to see which one is true.

Weak typing in JS is mainly from JS not having you be specific every time you list a variable. As we do not need to list out as a number or string, this makes it a weak typing. Other languages make you declare a number, or string, which makes it to be strong typing.

## Truthy and Falsy Values

These are fales that will either always come out to false, or always come out to true.

### Falsy Values

If we declare our variable to be either `false`, `0`(only the number 0), `''`(means empty string), `100/'string'`(both are not the same), or an empty variable. All of these come out to be automatic false when using them as booleans.

### Truthy Values

If we declare our variables to be either `true`, `1`(any number besides 0), `'string with content'`, `100/10`(both are numbers). `'true'`(written as a string), or `'false'`(false written as a string).

All of these are examples of Truthy and Falsy for true or false booleans.

## Loops

### For Loops

Example:  
`for (let i = 0; i < 10; i++) {`  
&nbsp;&nbsp;&nbsp;&nbsp;`console.log(i);`  
`}`  

Initialization: `let i = 0`

Condition: `i < 10;`

Update: `i++`

This example of a for loop. What is happening is that i is being declared as 0. Since 0 < 10, it is true, runs console logs, then `i++` adds 1 to 0,and now `i` is declared as 1.  
This process runs over and over through until `i` is 11, then it becomes false, and exits out of the loop.

### While Loops

While loops are very simular to for loops. One of the main differences is that with a for loop, its more towards setting to something. A while takes in more of a boolean, which is true or false. If the while loop is true, it will keep going __UNITL__ it gets a false. Then it will break out of the loop.

## Key Loop Concepts

### Keywords

`break;`  
Means it will stop, not execute the rest of the loop, and *breaks* out of the loop. When we have reached what we want, or to stop something, this is nice because we can control how long the loop will go for if we do not want the whole loop running.

`continue;`  
Means if will stop the *current* code block it is in, test to make sure the loop can still go on, and start back on the loop it is in. Then runs again.  
This is very nice for examples when you want the local code to run just until that momment, dont run the rest of what is in that local code block, and then continue the loop if the loop is still true.

Example. Local code means if you are an if statement, and there is an else if or else after, it will not run the rest of the else if or else if the `continue;` or `break;` code is run.

## Resources

### From the Duckett HTML book

- Chapter 3: “Lists” (pp.62-73)
- Chapter 13: “Boxes” (pp.300-329)

### From the Duckett JS book

- Review from Reading 02 - Chapter 2: “Basic JavaScript Instructions” (pp.70-73)
- Chapter 4: “Decisions and Loops” from switch statements on (pp.162-182)

Please visit my Github for more of my Projects!

[Charlie Fadness Github](https://github.com/fadnesscharlie)
