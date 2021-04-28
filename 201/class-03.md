# Class 02

* [Home](https://fadnesscharlie.github.io/reading-notes201/) 

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