# Class 201 Reading Notes

* [201 Home](https://fadnesscharlie.github.io/reading-notes/201/)

## Images

Having your images be around the same size per category you set them in will help the pages load faster. Being able to load the images on the page and having the page save this space for the page will help load and render the images faster. Aligning images in the center of the screen using `display: block;` and `margin: 0px auto;`(this sets the top and bottom to 0px, and auto left and right) will make it have its own line, then display it in the middle of the page.

### Background Images

Placing a background image inside of an element or whole page is placed in CSS. Using: `background-image: url("images/example.gif");`

You can modify those images with 4 differnt property values.

* `repeat`
  * In repeat, we can `repeat-x` and `repeat-y` for the x and y axis.
* `no-repeat`
  * Does not repeat the image
* `fixed`
  * This fixes the image to that spot on the page and does not move with the page.
* `scroll`
  * The image will scroll with the page.

### Background Position

Background position is a pair value. Using: `background-position: center top;` is one example. You can mix and match `left`, `center`, and `right` but if you do not specifiy the second pair, then it will always default to center.

### Background Shorthand

With background short hand, it is simular to how you can use border short hand. You can use: `background: red url(image/example.gif) no-repeat top center;` Which tells us the color, url, repeat, and position all in one line for us. One thing to take note, is that this must be in the correct order.

1. background-color
2. background-image
3. background-repeat
4. background-attachment
5. background-position

You can concaitinate the image background with `background: url(image/example.gif) no=repeat top right, url(image/example.gif) no=repeat top left`

### Image Rollovers and Sprites

With image rollover, we can specify and change the image when the user hover over it, or clicked on it. By placing the pictures in line with each other, they in a way overlap each other, but when the user hovers, or clicks, those images come to the front and be the image that is displayed.

Having a base: `cssIdHere {}`, then using the `cssIdHere:hover {}`, inside of our code block we can set the image to I believe offset the other images, which will inturn take over the position of the previous image. The `cssIdHere:active {}` does the same, but when clicked the image that is inside this code block becomes the primary image.

### Gradients

<!-- https://www.w3schools.com/css/css3_gradients.asp Resource taken for updated code base-->
Using gradients we have to specify two fifferent colors we use the code: `background-image: linear-gradient(direction, color-stop1, color-stop2,...);`. The default will be the first color on top, and second color on the bottom. We can specify where we want this color to be by having the left be the start, using: `background-image: linear-gradient(to bottom right, red, yellow);`. We can see the colors will go from top left, and move diagonally to the bottom right.

### Contrast

Make sure when you are using a background image that you see the contrast of the image as it loads into the page to be able to understand and see the image or words that are in front or behind them. If the words are hard to read then changing those to make them better will make it more user friendly in the end.

## Practical Information

### Search Engine Optimization

SEO stems down to what makes your page relevent enough for search engines to make them a priority.

#### On-Page SEO/Techniques

Are things like keywords, and words users may use in the search engine to look for your site.

There are seven key places where kyewords can appear in order to improve your page's finability.

1. Page Title
2. URL/Web Address
3. Headings
4. Text
5. Link Text
6. Image Alt Text
7. Page Descriptions

In these seven places are where you want to place your keyword for a website to find you and make your page more popular then others.

#### Off-Page SEO/Techniques

This is how many sites link to your site, and how well those link up, what site content that is related to yours. Search engines will look through your code and try to find words of text that may relate to your site, one example would be, what words do you have in your `<a>` tag besides just click me.

### How to Identify Keywords and Phrases

There are six things you can do to help find which keywords best describe your website and what keywords and the right keywords for your site to display that will attract more users.

1. Brainstorm
  a. Write down a list of keywords you think will descibe your site, and talk with others as well, as their approach to your website will be different and they can look at it in a different angle then you might. Including phrases and not just keywords will help as well.
2. Organize
  a. Put things into categories and sections can help expand your page and let you be specific on those topics.
3. Research
  a. Researching online for other keywords and other words you can use instead. Just becareful not to go overboard as some other words may hurt instead of help you.
4. Compare
  a. Comparing keywords to other websites can be a way to find out which keywords best suit your needs. Being able to google and see how many search results certain keywords give vs other words can be a better way to make your page stand out from the others.
5. Refine
  a. Being able to dile down and narrow your words of choice can help. If a certain phrase or word is very popular, dont feel afraid to not use those keywords, just refine others, or see what other words can turn into phrases.
6. Map
  a. Choose a few of those keywords and place them on each page. Each page does not need to have every keyword you choose, as further away from your main page, the more specific your keywords should be.

### Analytics: Learning About Your Visitors

You can sign up for google analytics that can show how many people have come to your website, and even if they stay for a longer duration on one page, and move to another, that will cound as another visit instead of the same visit. Things to take into account is visits, unique visit, page views, pages per visit, average time on site, date selector, and exporting the information.

Where are you visitors looking at. Which pages do they arrive on, which page do they leave, sometimes it tells you if the users scroll through the whole page, or do they stop at a certain area and move on from there.

You can even see where they come from. From a directed website, referrer, or a link. Being able to see if they typed in the browser your website, or used a bookmark to access your page. There are tons more things that the page collects from you that they can use the track and better fine tune your website for more people and visitors.

### Domain Names and Hosting

Domain names is your url. The address that you want to use, there are millions of registered domain names and finding the right one may take a while.

Web hosting is a server that is always connected to the internet that stores your website there so people can access the website as long as the server is up and running.

### FTP

File Transfer Protocal which is used to transfer your files from your machine to the server. Once you register a hosting server you will be given instructions to load your files to the FTP. Given a username and password to access these files, it is strongly recommended to not let anyone gain access as then they can modify your website or load in other content from their machine.
