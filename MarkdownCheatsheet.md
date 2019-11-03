# My Markdown Cheatsheet 


# References
## Visual Studio Markdown Editor Extension

> [Notes Source](http://vsixgallery.com/extension/9ca64947-e9ca-4543-bfb8-6cce9be19fd6/)
[github](https://github.com/madskristensen/MarkdownEditor)

# Images
![Fig 2](11-Dynamicaly-change-the-view.png)


# Images OLD NOTES
### Drag and Drop from Solution Explorer
### Paste Image
Simply copy an image into the clipboard and paste it directly into the document.
This will prompt you for a file name relative to the document and then it inserts the appropriate markdown.


`<img src="../../../_Temp/parasha.png" alt="Parasha" />`

`<img src="AutoMapper02.png" alt="Shawn Wildermuth (screen shot 1)" />`

---

# Examples
> [Notes from github Cheatsheet](
https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
)

## Images
> See cheat sheet for more details on various type of  **images**.

> using the exclamation! mark
![Set Startup for MVC Default Page](images/Set-Startup-Default-Page.png)

## Lists
1. First ordered list item
2. Another item
  * Unordered sub-list. 
1. Actual numbers don't matter, just that it's a numbers (not working as I expected)
  1. Ordered sub-list (item 1)
  2. Ordered sub-list (item 2)
4. And another item.

   You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).

   To have a line break without a paragraph, you will need to use two trailing spaces.⋅⋅
   Note that this line is separate, but within the same paragraph.⋅⋅
   (This is contrary to the typical GFM line break behaviour, where trailing spaces are not required.)

* Unordered list can use asterisks
- Or minuses
+ Or pluses

## Code and Syntax Highlighting
- [source](https://support.codebasehq.com/articles/tips-tricks/syntax-highlighting-in-markdown)
### csharp
```csharp
public ActionResult Index()
{
	return View();
}
```
### bash
```bash
dotnet new sln # to create a sln file
dotnet new [template_name] -o [output path] # to create a project
dotnet sln [sln_name] add [csproj_name] # to add a project to a solutition.
```

Inline code e.g. `var vm = new IndexVM(id);` has **back-ticks** around it.

```csharp
var vm = new IndexVM(id);  // this looks better
```
[language list](https://highlightjs.org/static/demo/)

## Tables

> <sup> Note part of core Markdown spec but are used by GFM </sup>

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is    | centered      |   $12 |
| zebra stripes | are **neat**      |    $1 |
> The table above uses **:** to align the columns and it uses inline Markdown

### Rules

- There must be at least 3 dashes separating each header cell.
- The outer pipes (**|**) are optional
- you don't need to make the raw Markdown line up prettily. 


## Small and Tiny Font with sup and sub

1. combining **sup** and **sub** <sup><sub> Sample Text </sub></sup>
2. Just **sup**  <sup> Sample Text </sup>
3. Just **sub**  <sub> Sample Text </sub>

## Emphasis
- Emphasis, aka italics, with `*` or `_` *asterisks* or `_underscores_`.
- Strong emphasis, aka bold, with `**` or  `__` **asterisks** or __underscores__.
- Combined emphasis with `**` and `_`  **asterisks and _underscores_**.
- Strikethrough uses two tildes `~~`  ~~Scratch this.~~


## Blockquotes

> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.

Quote break.

> This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this is long enough to actually wrap for everyone. Oh, you can *put* **Markdown** into a blockquote. 

## Inline Html

### Definition list 
<dl>
  <dt>Term 1: dl, dt, dd</dt>
  <dd>Definition 1: Is something people use sometimes.</dd>
  
  <dt>GFM</dt>
  <dd>Github Flavored Markdown</dd>

  <dt>Markdown in HTML</dt>
  <dd>Does *not* work **very** well. Use HTML <em>tags</em>.</dd>
</dl>

## Horizontal Rule
Three or more hyphens (-), asterisks (*) or underscores (_)

## Line Breaks 
there is a difference between one and two (two make is like a paragraph)

More stuff on inserting YouTube videos


## Tasks
### Solar System Exploration, 1950s – 1960s

- [ ] Mercury
- [x] Venus
- [x] Mars
- [ ] Jupiter



# Keyboard shortcuts 
* <kbd>Ctrl</kbd> + **B** makes the selected text **bold** by wrapping it with **.
* <kbd>Ctrl</kbd> + **I** makes the selected text _italic_ by wrapping it with _.
* <kbd>Ctrl</kbd> + **Shift+C** wraps the selected text in a code block.
* <kbd>Ctrl</kbd> + <kbd>Space</kbd> checks and unchecks **task list items** 
  * see tasks example below
* **Tab** _increases_ indentation of list items.
  * kbd>Shift</kbd> + <kbd>Tab</kbd> _decreases_ indentation of list items.
* <kbd>Ctrl</kbd> + <kbd>K</kbd>, **C** wraps the selection with HTML comments.
  * <kbd>Ctrl</kbd> + <kbd>K</kbd> ,**U** _removes html comments_ surrounding the selection/caret.
* <kbd>Ctrl</kbd> + <kbd>PgUp</kbd> moves caret to _previous heading_
  * <kbd>Ctrl</kbd> + <kbd>PgDown</kbd> moves caret to _next_ heading

### Note, **kbd** is the HTML for expressing the Keyboard 
* Example: <kbd>Shift</kbd> + <kbd>F10</kbd>



# Tools
- [pandoc](http://pandoc.org/) convert files from one markup format into another, pandoc is your swiss-army knife. Pandoc can convert documents in markdown, 
1. HTML Formats including HTML slide shows, 
2. Word Processeors like docx ... OpenOffice ODT
3. Ebooks: EPub, ...
4. PDF (via LaTex), 
5. Lightweight markup formats:...
6. Custom formats: custom writers can be written in lua.
7. Other Documentation Formats, Page layout formats, Outline Formats, Tex Formats;


# Extensions
1. [markdown linkify verses](https://www.npmjs.com/package/markdown-linkify-verses)
2. Parse Bible references and replace with full verse text in Markdown, with Flexmark and Eden __Java__. [EdenFlexmark](https://github.com/JavaEden/EdenFlexmark)
3. [bible gateway](https://christianity.meta.stackexchange.com/questions/20/add-markdown-and-or-onebox-support-for-biblegateway)