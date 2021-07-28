# Forms and Events

- [201 Home](https://fadnesscharlie.github.io/reading-notes/201/)

## Forms

### Form Controls

There are a few types of form controls, they range from adding text, making choices, submitting forms, and uploading files.

### How forms work

When submitting inforamtion into your forms, that goes into a server, the server processes the information, and brings back something depending on what the inforamtion is programmed to put back.

It is based on a `name=value`. You should not change the name at all after its implemented to make sure it does not break anything down the road.

### Form Structure

All forms require an action, the value goes to an url page that reacts depending on the information sent.

method: get or post

Use Post when:

- Users will upload a file
- Is very long
- Contains sensitive data like passwords
- Adds information to, or deletes information from, a database

Use Get when:

- dealing with short forms
- Retrieving data from a web server only

### Input

`type="text"`
`<input type="text" name="username"/>`

Creates a sinlge-line text input, the `type` is what kind of information will be inputted, and the `name` is associated with what we want to do the information `name` when it gets entered.

`<textarea>What we display inside the text area for the user to see</textarea>`

<textarea>What we display inside the text area for the user to see</textarea>

In a `textarea`, this our comment section, we create a box that can hold multiple lines of text. Using JS we can remove the inforamtion we display inside the box for the user as they click inside the box.

Radio Button

Checkbox

Drop Down List Box

Multiple Select Box

There are a few ways to incorporate when we want the user to click or choose something. We can have a simple:

- Radio Button, which once, clicked can not be unclicked and only have one clicked per section.
- CheckBox, simular to the radio button, but with checks and the user can now select multiple or deselect their answer
- Drop Down List Box/Select Box, the user can see multiple choices and be able to scroll through information, as with the Radio Button, only one can be selected at time
- Multiple Select Box, simular to the Select Box, but here we can choose multiple items instead of just one.

Note that inside these button/boxes, we have values, values are the ones that will be shown to the user.

### Uploading and Sumbit

With File Input Box, we can upload a file from our local machine to send to the server.

Simular to that, the sumbit button does not upload a file, but a piece of information, simular to subscribing to an email list. You can add an image to the sumbit button by adding an `src=""` inside the input tag.

Labeling form controls are a way to incorporate multiple forms togather, and being able to use the `for` keyword to then link to what form it used in through the id/name tags for buttons.

Grouping form elements is for when collecting lots of information that you want to place all one section, being able to have everything all together with a legend that defines everything.

With HTML5 implementing, they have made some short cuts for adding form validation, adding dates, emails, urls, and search boxes. These boxes work with the browser and not just the JS to be responsive.

## Lists, tables, and Forms

### Lists

When creating lists, you can customize and make it more user friendly. By choosing the bullet point styles, and being able to place them inside or outside can customize your page better. Even having an image instead of the bullet can spice things up as well.

There is short-hand for placing the list style inside or outside the text.

### Tables

In our past readings we went over the concept of tables. To add some more on the styling and control aspect of it, ill briefly explain those.

Being able to change the heading to be able to style in a way that pops out and create the symbol of header, adding padding to cells to make it more readable, adding shading for alternate rows for readability, aligning number to one side to distinguish high and lower numbers.

Empty cells can be shown(`empty-cells: show;`), hidden(`empty-cells: hide;`), or inherit. Habing Gaps betweens cells using `border-spacing:` or `border-collapse: collapse;`.

More things to take note: Style your forms, buttons, text inputs, and legends!!!!

## JavaScript

With events, there are many ways of wrapping your mind and how to code it through.

Starting with how the event is processed. First when we start to look at the event, we can control what the event is, and most importantly what happens when the event is fired. From there, our code gets sent to another page, that runs a scripp based on what is send through. From being able to respond back with a certain line of text, or being able to start a program.

Event listeners are one of many things taht we can look towards for events. It can run multiple functions for one event, and have a focus like blur. Blur is a type of focus that when the user moves away from it, it blurs, which then we can set to fire and run our set of code.

One thing that we have to work around, is that event listeners do not take in parameters. Which can be an issue so working around this your code and having it do certain things takes more skill then the usual function.

Event flow is very important, its how we can tell the webpage or program when/where to start, stop, and return something. Understanding the flow will help becuase you are able to then be certain on when your function/progams will run and where to place the outcomes.

WIth mouse and key presses, you can set and control when something is clicked in a certain area that may now have a special property, or when something is typed that may not be in a text box. Being able to control these is like being able to use the copy and paste controls and clicking away from something that then responds in a way that you want.

With all of these together, we can now make our pages a lot more interactive and responsive in ways that we want, and have certain thing happen when someting is clicked, submitted, typed, focused, or even blurred away from something.

## Resources

### From the Duckett HTML book

- Chapter 7: “Forms” (p.144-175)
- Chapter 14: “Lists, Tables & Forms” (pp.330-357)

### From the Duckett JS book

- Chapter 6: “Events” (pp.243-292)

Please visit my Github for more of my Projects!

[Charlie Fadness Github](https://github.com/fadnesscharlie)
