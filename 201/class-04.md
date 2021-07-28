# HTML Links, CSS Layout, JS Functions

- [201 Home](https://fadnesscharlie.github.io/reading-notes/201/)

## Links

When we want to Link an image, we want to use the `<a></a>` tag. We use the link tag like so: `<a href="directory-of-web-location">Name/Description of Website</a>`.

`<a href="google.com">`  
This is our **opening tag**. We have our website link to where we want to be redirected when the user clicks on the link.  
In the middle of our tag, we have the name, desciption, or image. Basically what the user will click on. We want to make sure that whatever we use, whether that be an image or a description, we want the user to have a good idea of what it is before they are clicking on it. You wouldn't want to be rediected to a car dealership while searching for recipes now would you? I know I don't.  
`</a>`  
We use our closing tag to make sure that the link knows where to stop and end.

When you are linking to a website. Make sure that is the full website. We want to use the **Absolute URL**.

### Linking to Other Pages on the Same Site

When we want to link to another site within the website. We do not have to add the whole website from the beginnig. All we add the file name, and direction to that file. An example of this would be `<a href="about-us.html">About Us</a>`. Here we can see that it's very short and to the point.

The main concern while doing this, is making sure that you have right direction. When moving through your folder, you need to know if you are going to a parent, child, grandparent, or grandchild. This makes it easier for us to understand where we want to go. As we know how the basic understanding of grandparent/parent/child structure goes, we use this as if we are in the parent folder, and we want to move the child folder. That means we have to move out of our folder, find the child folder, go into the folder of the child, and now find the file. That can look something like this. `<a href="../aboutUsFolder/about-us.html">About Us</a>`. While inside of our parent folder, we use `..` to signify go out of, `/` means go in now we are inside the `aboutUsFolder`, and all we do now is signify that we want to go inside our about us page `/about-us.html`.

This is a small example of how we want to move through our folders as when we have more folder, our *direction* can get long.

### Email Links

Linking to an email is about the same thing. We use the same tag, just different directions. An example would be: `<a href="mailto:Sarah@example.com">Email Sarah</a>` We click on Email Sarah to start sending Sarah an email.

### Links to a New Window

Linking to a new window the same procedure, the main difference is that you adding a target. Example would be: `<a href="google.com" target="_blank">Google</a>` You can see all we do is just add the target attribute. <a href="google.com" target="_blank">Google</a> Try it out!

### Linking to a specific part of the page

We can add a `#` and the `id` of which tag you want to go to. Say your webpage is very long, and you want a link that takes you to the top. We can achieve this by first placing the id tag. `<h1 id="top">Top of the page<h1>` Then, at the bottom of the page `<a href="#top">Top</a>`.

We can do this to other webpages as well. `<a href="google.com/#top">Top</a>` This will take up to the top of the page google. Make sure you have the right tag to go to.

## Layout

### Building Blocks

Every HTML element that we have on our pages, CSS treats them as its own box. It seperates them between two differeny blocks. They will be either block-level box or an inline box.

Block-level boxes will start on a new line, seperated from other lines. Examples of some tags that this points towards are: `<h1><p><ul><li>`. While inline boxes flow inbetween the surrounding lines. Examples of these would be: `<img><b><i>`.

### Containing Elements

If you have a block-level box inside of another block-level box. The outer box will be the parent in this case, and wise versa for the boxes inside as the child. The most outer box, besides the body, will most likely be the containing element. While you can have multiple block-level boxes inside of each other, the most outer **containing element** will always be the direct parent.

## Postioning Elements

### Normal Flow

In a normal flow, the flow will be normal. Means that each box will be directly below the next with some spacing, stacking on top to make our webpage. Each box gives distance inbetween each box to make a sign of seperation. This is the basic understanding of how the webpages will be. Since our webpages have this be default we do not need to add the `position: static;`.

### Relative Position

Relative position means that one or more of the boxes have now moved, whether that be up, left, right, or bottom. It has shifted away from where it would be normally. When you add `position: relative;` this makes the webpage still do as it should. When you move something, the way the page is generated will still be the same and the position will be similar to normal flow but with offset elements.

### Absolute Position

In absolute position, we will have a box that will be positioned where we place it. This ignores the rest of the normal flow and overlapps them. This ignores the rest of the normal flow of the website. For our element, we use the code: `position: absolute;`. Make sure to be specific one where you want this element to sit and how it also effects visability and usability of the website.

### Fixed Position

In fixed position, we will have a box that will be positioned where we place it. This ignores the rest of the normal flow and overlapps them. As the user moves through the webpage, it will stay at its position no matter where you are on the webpage. For our element, we use the code: `position: fixed;`. Make sure to be specific one where you want this element to sit and how it also effects visability and usability of the website.

### Overlapping Elements

Overlapping elements use the z-index. The code base for this is `z-index: 10;`, 10 being 100% overlap over the rest of the content. Using this and fixed position can create your text to show over the other elements of the webpage and stay on top, or "bring to front" in other words. When using multiple z-index's, you can layer them as if you had one at 5, the one with 10 would overlap that one.

### Floating Elements

We can float elements as well, this wrapps the normal flow around this floating element like a current flows around a bolder in the river. Mainly it will either be on the far left or right on the page. It is recommended to add a width to your floating object as if you do not, sometimes it can take up the width of the webpage, creating normal flow with an offset image.

### Multiple Floating Elements

When dealing with multiple elemets that are floating, what can happen is that, some elements can sit in places that you do not want them to sit. Instead of having three side by side elements, what could happen is three sitting side by side, and then the next line only has two, while the last one is floating somewhere randomly where it sits. To solve this, we can add in the code: `clear:left`, `clear:right`, `clear:both`, or `clear:none`. This tells the element that nothing in the **same containing element** can touch this side of the listed **clear** element. If we want something to float and could possibly move due to page size, we add **clear** to make sure that no matter what happens on the page, nothing in the same containing elements can be on that side.

### Parents of Floating Elements

When containing elements that have just floating elements. Adding a border around it can be very difficult because the browser treats it as if it is zero pixels tall. This creates a simple border around floating elements be a simple compressed line that is zero pixels in height. To fix this, we add `overflow:auto` and `width: 100%;`

### Floating Columns

Floating columns can achieved by using float, setting your width, and a small margin to creat some distance between the floating elements. You can size your columns to be exact, setting a percentage to achieve perfect seperation no matter the webpage width, or just taking the math out of. If you doing 5 colums, it would be easier to do `width: 20%;` then dividing 960 by 5.

### Fixed vs Liquid Layouts

When using the fixed vs liquid layouts. Both have their ups and down, and its based towards your user audience. Fixed sites are very good for the purpose of users that have around the same pixels of a desktop. While liquid is better if they are using a tablet or phone as elements can shift due to the different pixels on the screen depending on if the screen is bigger or smaller.

## Linking Multiple Style Sheets

When you want to link multiple style sheets there are two options to choose from. The most basic is just linking multiple CSS stylesheets to your HTML file. The other way is to link other style sheets directly to your CSS stype sheet. This uses the following code: `@import url("link-to-CSS-style-sheet");` Note that if using this method, it needs to be linked above all other style rules. Many people do this, to control either a section, table, nav, and much more to control what content is showed on what page.

## Functions

The format of a function is below. We look at the function, what we want to call the function `sayHelloWorld()`, we can name this whatever we want. The main goal is to make sure the name relates to the function for better user ability. If we called it `pumpkingPieRecipe()` when we called it later, we would think it would relate to pumpkings, and not just writing Hello World for us.

`function sayHelloWorld() {`  
&nbsp;&nbsp;&nbsp;&nbsp;`document.write('Hello World!');`  
`}`

`function` is the function keyword.

`sayHelloWorld()` is our function name. We can name this whatever we want.

`{`  
&nbsp;&nbsp;&nbsp;&nbsp;`document.write('Hello World!');`  
`}`

This is our code block. Our list of commands of what we want the function to do for us.

### Parameters

`function sayHelloWorld(parameter) {`  
&nbsp;&nbsp;&nbsp;&nbsp;`document.write('Hello World!');`  
`}`

In functions, we can state a parameter, and when we call the function, we will need to add a parameter when we call it.

`sayHelloWorld(addParameterHere)`

### Calling the function

You can call the function as many times as you want

`sayHelloWorld();`

Group set of statements or instructors together to perform a specific task

Offer a way to store the steps

### Return keyword

In a function, we use the `return` keyword to return what the function has done. When the function does something for us, we need it to give us what it has done. That is what the `return` keyword does. If we give it parameters, we will get the parameters from the return key.

## Example Function

`function getArea(width, height) {`

&nbsp;&nbsp;&nbsp;&nbsp;`return width * height;`

`}`

When calling the function:
`getArea(7,8);`

The `7` is the width and the `8` is the height
This is called perameters
You can use arguemtns as variables as well.

In this case it would be `wallWidth = 7;` and `wallHeight = 8;`
This is called arugments

`getArea(wallWidth, wallHeight);`

## Pair Programming

In pair programming, you not only get to work with someone, but hone a set of skills that would otherwise not be offered to you if you did not. These skills are: Listening, Speaking, Reading, and Writing. Because you are either the "driver" or the "navigator" you have to hone these skills. Knowing what words to say, when to say them, how to inform the other person, and getting another perspective on someone else's code and how their mind may work adds to your set of skills to develop yourself in ways that would not possible if you only coded alone.

- Driver: The person that is coding, and only person typing code into the project. This person is writing code efficently using the information from both parties to optimize the code.
- Navigator: The person looking over the code for typos, bugs, and thinking of what can go next and where this project is going. Also is doing research ont he side to help more results and information in a short amount of time.

The efficeny of pair programming can take slightly longer in speed, but returns higher quality. This leads to less bugs, less troubleshooting, and a higher satisfaction for the client. Because you have two minds on one project going at the same pace and speed, one person is constantly thinking of where this code will go, checking for typos and bugs while the other person is coding away, bringing those ideas to paper and writing it out using both suggestions for the most optimal set of code in the allowed time.

In the new work field, a lot of training can be done over pair programming. Since we are already doing this method at CodeFellows, we are ahead of the game in this aspect as we already have these skills refined and ready for workplace environment.

## Resources

- [6 Reasons for Pair Programming](https://www.codefellows.org/blog/6-reasons-for-pair-programming/)

### From the Duckett HTML book

- Chapter 4: Ch.4 “Links” (pp.74-93)
- Chapter 15: “Layout” (pp.358-404)

### From the Duckett JS book

- Chapter 3 (first part): “Functions, Methods, and Objects” (pp.86-99 ONLY)

Please visit my Github for more of my Projects!

[Charlie Fadness Github](https://github.com/fadnesscharlie)
