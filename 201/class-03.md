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

### Limited Height