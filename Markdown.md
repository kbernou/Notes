# Markdown Reference Sheet

## Headers
Using headers liberally and sectioning out notes like that is beneficial for organization. 1 and 6 should be used sparingly.

```md
# Header 1
## Header 2
### Header 3
#### Header 4
##### Header 5
###### Header 6
```
# Header 1
## Header 2
### Header 3
#### Header 4
##### Header 5
###### Header 6

## Basic Formatting

`_italic_`: _italic_

`**bold**`: **bold**

`**_both_**`: **_both_**

`~~strikethrough~~`: ~~strikethrough~~

## _Italics_ are usable in headers. **Bold** in some.
#### _Italics_ and no **bold**

A horizontal rule can be created with `---` and an extra new line:

---

## Links
`[This](www.markdowntutorial.com)` is an inline [link](www.markdowntutorial.com). It is also where most of this was learned from.

[And of course **bold** and _italics_ work in here too](www.reddit.com)

Links can also be [pointed](./README.md) to other files.

#### And [links](www.google.com) work in headings

Reference links work by using two sets of square brackets, with the second set containing the name of a reference later in the document:
```md
Example [link][ref link 1]
...
[ref link 1]: https://github.com
```
Reference links can be referred to multiple times.

This is an example of a [reference link][ref link 1]

But look, we're bat at the [first][ref link 1] link!

Using `(#header-name)` as the [destination](#image-links) in the link allows you to jump to other places on the same page (witihn github at least).

[ref link 1]: https://github.com
[other-ref-link]: http://www.news.ycombinator.com

## Image Links

Inline image links with alt text is possible as well by prefacing the text portion with a `!`:

```md
![This is the alt text](https://upload.wikimedia.org/wikipedia/commons/0/06/Kitten_in_Rizal_Park%2C_Manila.jpg)
```

![This is alt text for an image link](https://upload.wikimedia.org/wikipedia/commons/0/06/Kitten_in_Rizal_Park%2C_Manila.jpg)
##### Image Credit: Kenny Louie from Vancouver, Canada [CC BY 2.0](https://creativecommons.org/licenses/by/2.0)

## Block Quotes

Starting a line with `>` creates a block quote

> It looks a little something like this

Over multiple paragraphs you must duplicate the `>`, including blank lines
> Multi paragraph quotes.
>
> They look like _this_. 
>
> Blank lines should get the ">" as well.

## Code
This is technically extended Markdown, but GitHub supports it and that's where these notes are going.

Inline code formatting is done by wrapping text with `` ` ``.

Code blocks can be created by wrapping the code with `` ``` `` (known as code fencing). Language can be included after for code highlighting, depending on the playform rendering the Markdown:

JS:
```js
    let foo = 1;
    let bar = 1;
    console.log(foo + bar);
```
Multiline code blocks can also be created by indenting lines with 4 spaces
     
     if (value == true) 
     {
         DoThing();
     }

## Lists

Unordered lists can be created by putting a `*` at the start of the line:
```md
* This be an _Unordered List_
* Put a "*" at the start of your line
* End up with this
```

* This be an _Unordered List_
* Put a `*` at the start of your line
* End up with this

Ordered lists can be achieved by using numbers instead:
```md
1. And here we have
2. An _Ordered List_
3. Just like writing normally
```

1. And here we have
2. An _Ordered List_
3. Just like writing normally

_Ordered lists don't even need to have the numbers increment. The following renders the same as above:
```md
1. First item
1. Second item
1. Third item
```

1. First item
1. Second item
1. Third item

However, the first number used in an ordered list determines the first number:
```md
5. First item
1. Second item
1. Third item
```
5. First item
1. Second item
1. Third item
   
Lists can be nested:
```md
* Nested Lists
    * Just use several more spaces than the parent element has
    * EZ PZ
        * Oh look, more depth
    * Back up one
* And back to the start
* Best practice is going no more than 3 levels deep
```

* Nested Lists
    * Just use several more spaces than the parent element has
    * EZ PZ
        * Oh look, more depth
    * Back up one
* And back to the start
* Best practice is going no more than 3 levels deep

Lists can also be multi-line and of mixed type:
```md
1. Lists can also be multi-line
 
    Simply add a space at the front plus an extra line (or a tab)


2. As you can see this works

    Works decently

    * Plus nested lists still work
    * So much nesting
```

1. Lists can also be multi-line
 
    Simply add a space at the front plus an extra line (or a tab)


2. As you can see this works

    Works decently

    * Plus nested lists still work
    * So much nesting

## Paragraphs and Breaks
A hard break requires a blank line between lines:
```md
A hard break

Looks like

this.
```
A hard break

Looks like

this.

Soft breaks require two spaces after each line:
```md
A soft break  
Requires  
2 spaces  
After each line  
Without the extra blank line
```
A soft break  
Requires  
2 spaces  
After each line  
Without the extra blank line

### List Interaction

The break rules apply to lists as well:

1. This is the first line of an ordered list, with two spaces at the end  
 This is one line  
 And this the next. 
 But all under one list item  
2. The double space can go at the end of the list item as well to produce the above

## References
[GitHub Markdown](https://guides.github.com/features/mastering-markdown/#intro)  
[Learn X in Y Mins](https://learnxinyminutes.com/docs/markdown/)  
[Markdown Tutorial](https://www.markdowntutorial.com) (Basic)  
[Adap P's Markdown Here Wiki](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)  