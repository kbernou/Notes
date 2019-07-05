# Markdown Reference Sheet

## Basic Formatting
_italic_

**bold**

**_both_**

A horizontal rule can be created with "---" and an extra new line:

---

## Headers

# Header 1
## Header 2
...all the way to...
###### Header 6

Using headers liberally and sectioning out notes like that is beneficial for organization. 1 and 6 should be used sparingly.

#### _Italics_ are usable in headers. **Bold** not so much

## Links

[This](www.markdowntutorial.com) is an inline link, and where the stuff in these notes was learned from

[And of course **bold** and _italics_ work in here too](www.old.reddit.com)

#### And [links](www.google.com) work in headings

This is an example of a [reference link][ref link 1]
This is another example of a [reference link][other-ref-link]
But look, we're bat at the [first][ref link 1] link!

Also you can [jump](#image-links) to other places in the same page (at least on Github).

[ref link 1]: http://www.github.com
[other-ref-link]: http://www.news.ycombinator.com

## Image Links

Inline image link with alt text is below (same as links but the text is prefaced with an "!"):
![This is alt text for an image link](https://upload.wikimedia.org/wikipedia/commons/0/06/Kitten_in_Rizal_Park%2C_Manila.jpg)
##### Image Credit: Kenny Louie from Vancouver, Canada [CC BY 2.0](https://creativecommons.org/licenses/by/2.0)

![Reference link example](ref)
[ref]: www.image.com

## Block Quotes

A block quote
> It looks a little something like this

Over multiple paragraphs you must duplicate the ">"
> Multi paragraph quotes.
>
> They look like _this_. 
>
> Blank lines should get the ">" as well.

## Lists

* This be an _Unordered List_
* Put a "*" at the start of your line
* End up with this

1. And here we have
2. An _Ordered List_
3. Just like writing normally

_Note_: Ordered lists don't even need to have the numbers places correctly. The following renders the same as above:

1. First item
1. Second item
1. Third item

* Nested Lists
    * Just use one more space than the parent element has (or a tab, depending)
    * EZ PZ
        * Oh look, more depth
    * Back up one
* And back to the start
* Best practice is going no more than 3 levels deep

1. Lists can also be multi-line
 
    Simply add a space at the front plus an extra line (or a tab)


2. As you can see this works

    Works decently

    * Plus nested lists still work
    * So much nesting

## Paragraphs and Breaks

A hard break

Looks like

this.

A soft break  
Requires  
2 spaces  
After each line  
Without the extra blank line

### List Interaction

1. The break rules apply to lists as well  
 This is one one line  
 And this the next. 
 But all under one list item  
2. The double space can go at the end of the list item as well to produce the above
 Otherwise you end up  
 with something like this.

 ## Code

 This is technically extended Markdown, but GitHub supports it and that's where these notes are going

 Inline code blocks are like `var this = true`, wrapped with "`"

 Multiline code blocks are indented with 4 spaces
     
     if (value == true) 
     {
         DoThing();
     }
    
Code "fencing" can be done by wrapping the block of code with "```"

```
if (value == true)
{
    DoThing();
}
```

Including the language right after the "```" will enable syntax highlighting
```javascript
if (value == true)
{
    DoThing();
}
```

## References
[GitHub Markdown](https://guides.github.com/features/mastering-markdown/#intro)
[Learn X in Y Mins](https://learnxinyminutes.com/docs/markdown/)
[Markdown Tutorial](https://www.markdowntutorial.com) (Basic)
