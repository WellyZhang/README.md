
# <a name='top'>Introduction</a>
This is a brief English introduction to `GitHub Flavored Markdown`, or `GFM`. Markdown has been adopted for its implicity and expressiveness over a wide range of applications and the specfic version from GitHub adds a myriad of extensions to it, only making it more than popular among programmers.

Now we are going to explore a little bit in depth of it.

Note that GFM also supports HTML.

## Headers
Use 1 ~ 6 '#'s to indicate header level. You can't really make a header bold, but you can italicize certain words(to be discussed later).

# Header One
## Header Two
### Header Three
#### Header Four
##### Header Fix
###### Header Six
###### _Italic Header Six_

## Text

### Italics
Surround words with underscores \_ to _italicize_ words.

### Bold
Surround words with two asterisks \*\* to make them **bold**.

### Combination of Italics and Bold
Surround with \*\*\_ like **_Italics and Bold_**.

### Straigh-through
Surround words with ~~ for ~~straight-through~~.

### Hightlight
Surround words with \` to `highlight`.

### Escape
Use \ for for escape.

### Newline
Use double blanks at the end of each line for soft break  
while use /n between lines for hard break such as

this.

## Links
Bear in mind that links could be combined with tricks from Headers and Text

### Inline Links
Wrap the text in bracets([]) and links in parenthesis(()) with optional floating "strings" seperated by a blank.  
If you still don't understand it, [**Google it**](http://www.google.com "Google").

### Reference Links
Here the link is actually a reference to another place in the document with the same contents as those in the parenthesis in the Inline Link grammer, impiled by the square brackets following the [text][text link].
[text link]: http://www.google.com "Google"

### Links in the Repo
Links could be incomplete with file-system-like paths such as  
[Emoji](./emoji.md) or [Emoji](emoji.md)

### Anchors as Links
Use HTML # to set anchors, for example your intention to return to the [top](#top) now.

## Images

### Images as Links
In GFM, images could be displayed by the Link grammer with a minor modification of a preceding !.  
But note here that text in square bracets would not be shown(so that component could be empty), and if you want to add links to your image treat the entire image grammer, the preceding ! included,  as text in the link grammar.
![First Father](http://octodex.github.com/images/founding-father.jpg "First Father")
[![Second Father](http://octodex.github.com/images/foundingfather_v2.png "Second Father")](http://www.github.com)

## Lists

### Bullet Points
Preface each line with an asterist \* to
* make  
* a  
* list.

### Grouping
To specify hierarchy, preface blanks. 
Plese note to indent one more space than the preceding one.
* to  
 * make 
  * it

### Numbering
\* could be replaced by a number following by a dot and a blank space. Similar hierarchy is also available, just remember every level starts with 1\.  

1. Place  
 1. Do not 
  1. Start with 1\.1  

### Task Lists
Task lists start with - and a space followed by a [], which if filled with x or a space.
- [x] Headers
- [x] Text
- [x] Links
- [x] Images
- [x] Lists
- [ ] Blockquotes
- [ ] Code Snippets
- [ ] Tables
- [ ] Emoji

## Blockquotes
> "To create a block quote, all you have to do is preface a line with the "greater than" caret (>). "  
>
> You can also place a caret character on each line of the quote. This is particularly useful if your quote spans multiple paragraphs.
>
> Notice that even blank lines must contain the caret character. This ensures that the entire blockquote is grouped together.

To ensure grouping hierarchy, precede one more \> than the previous level.
> such
>> as
>>> this

## Code Snippets
Warp your code with ``` and the programming language you use. As for me,
```Python
def emotion():
  print("I just love Python!")
emotion()
```
If you do not indicate the language you use, it will only be a darkened text block.

## Tables
Each entry should be seperated or enclosed by \|. Besides, headers are distinguished by ---- following in the next line also sepereated by \|. Note that entries could be images.
To sed alignmetn mode, append : on either or both sides of each entry.

| Name | Description |
| ------------- | ----------- |
| Help  | Display the help window.|
| Close | Closes a window.        |


| Left | Middle  | Right |
| :------------ |:---------------:| --:|
| col 3 is      | some wordy text | $1600 |
| col 2 is      | centered        |   $12 |
| zebra stripes | are neat        |    $1 |


| Image | Description |
| ---- | ---- |
|![Logo](http://img.chinatimes.com/newsphoto/2015-09-02/656/20150902001125.jpg "Google") | Google |

# Emoji
GFM supports Emoji naively. To display emoji, surround the name of the expression with two `:`s.  
E.g. `:blush:` :blush:  

GitHub has a [Emoji cheatsheet](http://www.emoji-cheat-sheet.com), but for your convenience I've also included it in the [repo](./emoji.md).

# Acknowledgement

I'm grateful for developers of [Markdown Tutorial](http://www.markdowntutorial.com/) which provides basics and fundamentals on how to write a startup Markdown file,  for his thorough explaination of GFM in Chinese and authors of the Markdown Cheat Sheet whose summarization is right to the point.
