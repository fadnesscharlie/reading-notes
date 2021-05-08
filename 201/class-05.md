# Class 201 Reading Notes

* [201 Home](https://fadnesscharlie.github.io/reading-notes/201/)

## Images

Having images on your site helps your site a lot. It shows or tells the user what the page might be able without even reading any context. When adding those images to your site, its best if you have a serpate folder called "images". When your site is larger, you can have sub-folders that hold more folders that are image categories.

### Links/images

Adding links and images are quite easy. It sometimes can be difficult to think of how your moving one image to another. In our mind, we just copy and paste right? Not so quite! But almost! In HTML we need to write where that link/image is coming from. One thing we must take note, '&copy' copywrite is a very big thing, especially around images, you can't copy every image you see on google and claim it to be your own, that's a big no no. Take note of how the image uses a self closing tag, while the link uses a opening and closing tag.  

We add our images in HTML by using the code: `<img src="Image_Adress" alt="Description of the image" title="More-info/tool-tip-info">`, this allows us to take an image from either our local machine, our repo, or a different website and post it here for us. You always want to include a description of what the image is in `alt=""`. That helps users with impaired vision understand the image, as sometimes it can read the description of the image out to them. A title is not nessessary, but nice to have when using a hover function.

Adding height and width is nice to an image. This is because when your loading a page, the page can load the rest of the text around the image while the image loads. Also placement, knowing where to place your image is a good tool to have. Understanding if you want your image as a block-level element, or if you want your image to be an inline with the rest of the text, or even in the middle of your text all together.

### Three Rules for Creating Images

The three rules:

* Save images under the correct format
* Save Images at the right size
* Measure images in pixels

Using these three rules, your image will load faster, will not be stretched, compressed, and know exactly how the image will turn out will it will be laoded on the page.

Look into Online Editors to edit and save images. Some weblinks are [photoshop.com](photoshop.com), [pixlr.com](pixlr.com), [splashup.com](splashup.com), and [ipiccy.com](www.ipiccy.com).

When wanting to know the image size, you can open the image into a new tab, this will tell you the exact pixels of the image.

### Figure and Figure Caption

With `<figure></figure>` and `<figcaption></figcaption>` we can add a caption for the image.

Here is an example, using the following code:

`<figure>`  
&nbsp;&nbsp;&nbsp;&nbsp;`<img src="https://images.unsplash.com/photo-1570639831023-bb6815023c5c?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1944&q=80" alt="Picture of a pumpkin"/>`  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`<figcaption>Here is the caption of the image, in here we can write out the description, or what it may be referenced or grabbed from</figcaption>`  
`</figure>`

<figure>
<img src="https://images.unsplash.com/photo-1570639831023-bb6815023c5c?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1944&q=80" alt="Picture of a pumpkin"/>
<figcaption>Here is the caption of the image, in here we can write out the description, or what it may be referenced or grabbed from</figcaption>
</figure>

## Colors

Brings your site to life. You can place color anywhere on the page you want, if you want to target just the text `color: blue;`, the block of text, background `background-color: red;`, border of an image `solid border: black;`, etc. It can make important things stand out and make your site come to life.

Picking out your color comes in three different types of ways. There is the actual word of the color "`color: red;`", a six digit code "`#ffffff`", and a RGB(red, green, and blue) number from 0-360 "`color: rgb(75,75,75);`".

## Contrast

Contrast gives light and darkness to certain areas and colors. Which bring additonal light or darkess to match the surrounding colors, making things pop or not.

## Opacity

There is a way to add opacity to a RBG as well. You choose your colors adding a fourth number at the end, ex. "`background-color: rgb(75,75,75,.5);`" Opacity is nice when you want to have a color fade into the background, or bring something else from the back.

## HSL Colors

HSL works with Hue, Saturation, and Lightness. 

* Hue is simular to the color wheel, it goes through numbers 0 and 360 picking which color you want.
* Saturation is the amount of gray in color, between 0% and 100%.
* Lightness is the amount of white(lightness) or black(darkness) in a color. 0% being white and 100% being black.  

Examples of this would be "`background-color: red; background-color: hsl(360, 100%, 50%);`" , you can add a fourth number between 0-1 to add opacity.

## Text

Each type of Text family has their own characteristics. Be sure to look around and see whats avaiable and see what meets your site and user needs.

### Weight

There are four different types of weights, starting with light, medium, **bold**, and black.

### Style

We can add style to our font, examples would be Normal, *Italic*, and *Oblique*.

### Stretch

You can even have types of stretch, they range from Condensed, Regluar, and Extended.

## Typeface

When using typeface, make sure it is installed on your local server, or imported or else it will not know where to grab these letters from.

To bring a font into your CSS, you use the following code with the examples:

`font-family: Times;`

Here are a few examples:

* Serif
  * Georgia
  * Times
  * Times New Roman
* Sans-Serif
  * Arial
  * Verdana
  * Helvetica
* Monospace
  * Courier
  * Courier New
* Cursive
  * Comic Sans MS
  * Monotype Corsiva
* Fantasy
  * Impact
  * Haettenschweiler

### Specifying TypeFaces

When adding a typeface to your site, its common practice to list a few if you are using outside of the common typefaces listed on your local machine. We add our typeface we want the user to see first, then add additional behind it as *backup*. This makes it simple in case the user does not have your typeface, a font will still be chosen besides the default/generic fonts listed above. If a font name has more then one word, it is best pratice to use "double quotes".

### Font sizes

There for several ways to declare a font size, the three most common, is: pizels, percentages, and em. Pixels make it so you can control the size of the words precisely, percentages have a default of 16px at 100%, and an em is equivalent to the width of a letter m ot 1em which is 16px. The default font size of a text in a webpage is 16px.

### Font Weight

With font weight you can make things **bold**. This would be written as: `font-weight: bold`. You can use this while declaring multiple classes to make everything bold at once.

### Font Style

With font style, there is normal, *Italic*, and *oblique*. We write these like: `font-style: italic;`. Italic is a whole design with a slanted feature, while oblique is that font just slanted.

### Text-Transform

In text transform, here is where we can capitalize, uppecase, and lower back. We use these features with: `text-transform: uppercase;`, `text-transform: lowercase;`, and `text-transform: capitalize;`.

### Text-Decoration

In text-decoration, we can add and take away some things. Example of this would be when creating a link there is always a line underneath the link. With `text-decoration: none;` we can remove this line underneeath. We can use the same logic for `text-decoration: underline;`, to add a line underneath context,`text-decoration: overline;`, to add a line over top of the text and `text-decoration: line-through;`, to put a line through the text.

### Line-Height

In line height, we can add space above text. When creating the font size, that is the distance from top of the character to the bottom. With `line-height 1.5em;`, we can add space above the top of the character. This is used to seperate context and words from each other.
