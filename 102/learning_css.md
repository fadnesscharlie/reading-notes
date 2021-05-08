wdawawwdawAsdawAW1d3aawaawd dwawswwdsdwdewA%W!WsssawADAa4w3sw1wawswwdewwswawd
# Learning CSS

# Learning JavaScript Programming

[Home](https://fadnesscharlie.github.io/reading-notes/102)

![Image of Css](https://images.unsplash.com/photo-1505685296765-3a2736de412f?ixid=MXwxMjA3fDB8MHxzZWFyY2h8NHx8Y3NzfGVufDB8fDB8&ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60)

## Linking CSS File

There are 3 ways of adding CSS to your file. You can place your CSS inside your element, on your header, or link an external CSS style sheet.

While placing your CSS in your element seems fairly simple, you can see what CSS is being done to just that section, simple!

Adding CSS to your header. This makes it simple, head to the top of the page, and see all the CSS that is on that page.

Linking your CSS page. Why would you want to create a whole new page and have all your CSS there when you place it in your file? One big reason why is with an external CSS, you can create templates. And have CSS effect the same elements on different pages. You would not have to copy over every single CSS you made for that element on each page, and instead you can write one page, link the file, and the file will show the same CSS throughout all of your pages.

Finally, what happens if I wirte my CSS in my page, and the exrnal page. As the page is being read, we add the link to your CSS at the top, it then reads down from there, Only the bottom most CSS of any taged element will display.

## Elements

As its own box

There are rules in CSS, they contain two parts, a selector and a declaration. inside the declaration there is Property and a Value.

A selector would be:  
`p {`
    font-family: Arial;}

A declaration would be:  
p {
    `font-family: Arial;}`

Inside the declaration there is a property and a value:
The property is:  
p {
    `font-family:` Arial;}

The value is:  
p {
    font-family: `Arial;}`

## Seclectors

There many differnt types of selectors, from:

* `universal: * {}`
* `type: h1, h2 {}`
* `Class: .note {}`
* `ID: #Instroduction {}`
* `child: li>a {}`
* `descendant: p a {}`
* `adjacement sibling: h1+p {}`
* `general sibling: h1~p {}`

## Colors

Brings your site to life. You can place color anywhere on the page you want, if you want to target just the text, the block of text, background, border of an image, etc. It can make important things stand out and make your site come to life.

Picking out your color comes in three different types of ways. There is the actual word of the color "`color: red;`", a six digit code "`#ffffff`", and a RGB number from 0-360 of red, green blue "`color: rgb(75,75,75);`".

## Contrast

Contrast gives light and darkness to certain areas and colors. Which bring additonal light or darkess to match the surrounding colors, making things pop or not.

## HSL Colors

HSL works with Hue, Saturation, and Lightness. hue is simular to the color wheel, it goes through numbers 0 and 360 picking which color you want.

Saturation is the amount of gray in color, between 0% and 100%.

Lightness is the amount of white(lightness) or black(darkness) in a color. 0% being white and 100% being black.  Examples of this would be "`color: hsl(360, 100%, 50%);`", you can add a fourth number between 0-1 to add opacity.

## CSS3 RGBA

There is a way to add opacity to a RBG as well. You choose your colors adding a fourth number at the end, ex. "`background-color: rgb(75,75,75,.5);`" Opacity is nice when you want to have a color fade into the background, or bring something else from the back.

[Charlie Fadness Github](https://fadnesscharlie.github.io/Reading-notes/)
