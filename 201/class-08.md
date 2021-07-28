# More CSS Layout

- [201 Home](https://fadnesscharlie.github.io/reading-notes/201/)

## Layout

Here we will go over Layout again, as a refresher and look to see what we can incorporate now that we did not know much of before.

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

## Resources

### From the Duckett HTML book

- HTML/CSS book, Ch. 15, “Layout” (again; repeat of Class 4 reading)

Please visit my Github for more of my Projects!

[Charlie Fadness Github](https://github.com/fadnesscharlie)
