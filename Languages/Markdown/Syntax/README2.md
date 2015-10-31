Markdown(Extra) Cheat Sheet

Blockquotes(Ctrl+Q)
Code Block
Emphasis
Headers
Horizontal rules
Images(Ctrl+Shitf+L)
Inline Html
Links(Ctrl+L)
Lists
Paragraph
Table
Literal Characters
Footnote
Math
Multi-Markdown
Blockquotes
ShortCuts: Ctrl+Q



Markdown uses email-style > characters for blockquoting.
> This is a blockquote

Code Block
Indent 4 spaces or 1 tab

This is a normal paragraph:

    This is a code block.
or (code syntax highlight)

```javascript
for(var i=0; i<100; i++)
    console.log("Hello, MdCharm");
```
Result:

for(var i=0; i<100; i++)
    console.log("Hello, MdCharm");
or

~~~~~~~~~~~~~~~~~~~~~
Here is the code
~~~~~~~~~~~~~~~~~~~~~
Emphasis
Shortcuts	Syntax	Result
Italic	Ctrl+I	*italic* or _italis_	italic
Bold	Ctrl+B	**bold** or __bold__	bold
Strike through	Ctrl+T	~~Strike through~~	Strike through
Headers
This is an H1
=============

This is an H2
-------------
or

# This is an H1

## This is an H2

###### This is an H6
Header Id Attribute

## Header 2 ## {#header2}
or

Header 1 {#header1}
========
Link back to header

[Link back to header 1](#header1)



Horizontal rules
* * *

***

*****

- - -

---------------------------------------

_ _ _
Images
Markdown Input	Result
![MdCharm](qrc:/mdcharm.png "MdCharm")	
width and height attribute
Please enable Multi-Markdown first.

![MdCharmWH][]

[MdCharmWH]: qrc:/mdcharm.png width=100px height=100px
result


MdCharmWH
Inline Html
This is a regular paragraph.

<table>
    <tr>
        <td>Foo</td>
    </tr>
</table>

This is another regular paragraph.
Links
Markdown Input	Result
This is [an example](http://example.com/ "Optional Title") inline link.	This is an example inline link.
<http://example.com/>	http://example.com/
Lists
Unordered lists
Asterisks, plus signs or dashes:

* Red
* Green
* Blue

+ Red
+ Green
+ Blue

- Red
- Green
- Blue
Ordered lists

1. One
2. Two
3. Three
Paragraph
One or more consecutive lines of text
separated by one or more blank lines.

This is another paragraph.
Line Break
To create a line break, end a line in a paragraph with two or more spaces

Table
First Header  | Second Header
--------------|--------------
Content Cell  | Content Cell
Content Cell  | Content Cell
or

|First Header  | Second Header|
|--------------|--------------|
|Content Cell  | Content Cell |
|Content Cell  | Content Cell |
Left aligned

| Item     | Value |
|----------|:------|
| Computer | $16   |
Right aligned

| Item     | Value |
|----------|------:|
| Computer | $16   |
Center aligned

| Item     | Value |
|----------|:-----:|
| Computer | $16   |
Literal Characters
from http://daringfireball.net/projects/markdown/syntax#backslash

Markdown allows you to use backslash escapes to generate literal characters which would otherwise have special meaning in Markdown's formatting syntax. For example, if you wanted to surround a word with literal asterisks (instead of an HTML <em> tag), you can backslashes before the asterisks, like this:

\*literal asterisks\*
Markdown provides backslash escapes for the following characters:

\   backslash
`   backtick
*   asterisk
_   underscore
{}  curly braces
[]  square brackets
()  parentheses
#   hash mark
+   plus sign
-   minus sign (hyphen)
.   dot
!   exclamation mark
Footnote1
Footnote example[^footnote].

[^footnote]: I am a footnote.
Math
Please enable Multi-Markdown first.
Export to PDF, ODT and Live Preview are not supported
form: http://fletcher.github.com/peg-multimarkdown/#math

HTML Header: <script type="text/javascript"
src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML">
</script>

An example of math within a paragraph --- \\({e}^{i\pi }+1=0\\)
--- easy enough.

And an equation on it's own:

\\[ {x}_{1,2}=\frac{-b\pm \sqrt{{b}^{2}-4ac}}{2a} \\]

That's it.
Multi-Markdown
Enable Multi-Markdown: Select Settings -> Preference... -> Environment, change Markdown Engine to MultiMarkdown

I am a footnote