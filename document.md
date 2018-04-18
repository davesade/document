# First level
To create main description, you simply use `#` to mark down initial name of the chapter.

## Second level
As you can see in the sidebar, lines beginning with `##` are considered as chapters and automatically populated to create list of contents.  

### Third level
Depending on your settings, `###` are still acting as a sub-chapter, but it is not shown in sidebar. Have a look at `index.html` file. This is where you configure, how many levels will be displayed by sidebar.  

#### Fourth level
Does it even exists? :)

## Examples of MarkDown syntax
MarkDown itself is very simple.  
`*italic*` will result *italic*.  
`**bold**` will result **bold**.  
Use `>` to create quotes like this:  
> Some famous quote.  
> Written by:  
> Cicero  

Create a divider line by putting `---` or `***` or `___` to your document:  
***

Lists can be achieved simply by putting `-` or `*` or `+` at the start of the line, have a look:  
- Apples
- Pears
- Oranges
- Bananas
- Grapes

Alternatively, you can create numbered lists simply by putting numbers on start of the line.  
1. First
2. Second
3. Third
4. Fourth
5. Fifth

## Tables

Simple tables are also possible in MarkDown, see below:  

| Tables           | Are           | Cool  |
| ---------------- |:-------------:| -----:|
| Last column is   | right-aligned | $1600 |
| Middle column is | centered      |   $12 |
| I like beer      | and nuts      |    $1 |

And the source code looks like this:  

```
| Tables           | Are           | Cool  |
| ---------------- |:-------------:| -----:|
| Last column is   | right-aligned | $1600 |
| Middle column is | centered      |   $12 |
| I like beer      | and nuts      |    $1 |
```

## Other examples

There is much more to learn! For example, there are also some flavours of MarkDown (ie. [Github flavoured MarkDown]()), allowing you to do more. Figure out by our own, how the source code of following examples looks like:  

!> **Time** is money!

?> *TODO* list

* [x] first
  * [x] one
  * [ ] two
  * [ ] three
* [x] second

Please continue with sidebar table of contents to explore more options.  

BTW this is file `document.md`, when you look inside repository.
