Basics of Markdown syntax:

**Headers**: Use the **#** symbol to indicate headers. The number of # symbols indicates the level of the header (h1 - h6).

# H1

## H2

### H3

#### H4

##### H5

###### H6

**Emphasis**: Use * or _ for italics and ** or __ for bold.

*This text will be italic*
_This will also be italic_

**This text will be bold**
__This will also be bold__

**Lists**: For unordered lists, use * or - or +. For ordered lists, simply number the items.

Unordered:
* Item 1
* Item 2
  * Item 2a
  * Item 2b

Ordered:
1. Item 1
2. Item 2
3. Item 3
   * Item 3a
   * Item 3b


**Links**: Use this format [text](URL).

[GitHub](http://github.com)

**Images**: Very similar to links but with an exclamation mark before the square brackets. Format: ![Alt Text](url).

![GitHub Logo](/images/logo.png)
Format: ![Alt Text](url)

**Blockquotes**: You can indicate blockquotes using >.

> This is a quote.

**Code Blocks**: Indent your code by four spaces or use triple back-ticks (```) to create a code block. For syntax highlighting, specify the language right after the opening three back-ticks.

```javascript
function test() {
  console.log("look ma’, no spaces");
}
```

```

To see the result of your Markdown file in VS Code, use the "Open Preview" button in the top-right corner or use the shortcut Ctrl + K V. Remember, every platform that uses Markdown has a slightly different implementation. The above examples should work in most cases, but there may be exceptions.

There are many more advanced features to Markdown such as tables, task lists, etc., that you can learn once you've mastered the basic.
