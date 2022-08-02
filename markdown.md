# Markdown basics, tips and visual editor

## Markdown cheat sheet

```
| Markup syntax    | Name                        | Description & Examples                          |
|------------------|-----------------------------|-------------------------------------------------|
| #                | Heading 1<h1>               | # Article title or the main heading             |
| ##               | Heading 2<h2>               | ## Subtitle or as I like to call "heading 2"    |
| ###              | Heading 3<h3>               | ### Do you get the point, right?                |
| ####             | Heading 4<h4>               | #### This is rare, but can happen               |
| #####            | Heading 5<h5>               | ##### Never seen one                            |
| ######           | Heading 6<h6>               | ###### Stop! Don't you even think...            |
| **bold**         | Bold                        | This is an **bold** example                     |
| *italic*         | Italic                      | This is an *italic* example                     |
| ---              | Line<hr>                    | Just a line break (*** ___ are alternatives)    |
| >                | Quote/Comment               | > Comment styled line                           |
| *                | Unordered list item         | * List item (- + are alternatives)              |
| 1.               | Number ordered list item    | 1. Just like this!                              |
| a.               | Character ordered list item | a. Nice to use inside and number ordered list   |
| - [ ] text       | Unmarked to-do list item    | Create to-do lists                              |
| - [x] text       | Checkd to-do list item      | This one is a checked [✔] box                   |
| ```code```       | Code                        | ```Code styled line/block```                    |
| [text](URL)      | Hyperlink                   | [Download here!](https://google.com)            |
| ![alt text](URL) | Image                       | ![profile pic](https://github.com/petry078.png) |
| \                | Disable Markdown style      | Works with:  ``` * # - + !                      |
|==================|=============================|=================================================|
|                  |                             |                                                 |
| |Table           | Column         | Another column      | How many you need  |                   |
| |----------------|----------------|---------------------|--------------------|                   |
| | Table item     | Column item    | Another column item | This is a md table |                   |
```

## Tips

* On VS Code, you can open the preview tab with `cmd + shift + V`;
* Drag the preview tab to the right until you see it trying to divide the screen in two.
* Make sure you have a white space " " after a markup symbol;
* Always test if it works on your environment. Not every browser or website renders all Markdown styles;
* Markdown accept HTML tags. So if you can't make it with native Markdown, use HTML tags (this includes CSS and JavaScript);
* It is important to edit Markdown using monospaced fonts. Like the VS Code standard, Courier New or Roboto Mono.
* Keep a black line after a marked one. For example:

  > Example

  Just like this!

## Markdown Editor

Markdown can be intimidating at the beginning. Here is how to get started with the visual Markdown Editor:

* [Download here!](https://marketplace.visualstudio.com/items?itemName=zaaack.markdown-editor)
* Install the extension on VS Code;
* Right-click the file you need to edit and select `Open with markdown editor` or type `alt + shift + cmd + M`.

### Markdown Editor: usage

* Show the menu bar.
* If you use light themes on VS Code, you need to adjust this at `... > Content Theme Preview`
* You can copy & paste text with links and styles (and pictures) from Google Docs and every other web pages.
* If you copy an image from the web, it will create a markup with the image link.
* If you copy an image from your computer it will automatically save the image inside assets `assets/like-this.png`
* There are emojis! Type : and search for what you looking for. 👊 🏠 🏁 👌 🚀️
* Home and End keyboard button doesn't work. :/ But you can use `cmd + arrow keys` and `alt + arrow keys` to jump through words.
* You can export to HTML.

### Markdown Editor: problems

* Lists doesn't work really well. The buttons to add lists can break others lists, and it will always add a black line on top of the list.
* Creating tables inside the visual editor is nice and easy, but it will break the original Markdown file.

## Conclusion

The Markdown Editor by zaaack works fine and can be very useful in cases you need to copy and paste marked content from the web and don't have time to mark every thing again. But you still need to edit the raw .md file before pushing it to GitHub.

[Visit this GitHub documentation about Markdown to learn more.](https://docs.github.com/pt/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
