# Class 201 Reading Notes

* [201 Home](https://fadnesscharlie.github.io/reading-notes/201/)

## Local Storage

### HTML5 Storage

Most things that we will be doing will use HTML5 storage. This was made as a fix to have something that is accessiable for everyone and most browsers to move away from cookies that would just slow down your web speeds. HTML5 Storage is based on key value pairs. Everything is stored as strings, so if you want to return back a number, you need to set it as a number or floating numbering depending on what you want to do. When we want to 

### Storing Information

While storing information, we store them in key value pairs.

`localStorage.setItem('key', 'value');`
`let storedItem = localStorage.getitem('key');`
`console.log(storedItem);`

This will return `'value'` for us.

#### Square Bracket Syntax

In square brackets, we are taking out the getItem and setItem for a specific syntax.

`localStorage["key"] = value;`
`let storedItem = localStorage["key"];`
`console.log(storedItem);`

This will return `'value'` for us. This is the same thing, but with a shorter syntax.
