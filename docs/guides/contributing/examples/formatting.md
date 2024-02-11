# Formatting

This page will go over extra typography features. If you're not familiar with Markdown, it's best to read [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#headers)


[Critic Markup](https://github.com/CriticMarkup/CriticMarkup-toolkit) can be used, which adds the ability to highlight suggested changes, as well as add inline comments to a document:

![](img/formattingworkaround.png){.center}

Text can be {--deleted--} and replacement text {++added++}. This can also be
combined into {~~one~>a single~~} operation. {==Highlighting==} is also
possible {>>and comments can be added inline<<}.

{==

Formatting can also be applied to blocks by putting the opening and closing
tags on separate lines and adding new lines between the tags and the content.

==}

---
### Highlighting Text

Text can be highlighted with a simple syntax, which is more convenient that directly using the corresponding `mark`, `ins` and `del` HTML tags:

```
- ==This was marked==
- ^^This was inserted^^
- ~~This was deleted~~
```

- ==This was marked==
- ^^This was inserted^^
- ~~This was deleted~~

---
### Sub and Super Scripts

Text can be sub- and superscripted with a simple syntax, which is more convenient than directly using the corresponding `sub` and `sup` HTML tags:

```
- H~2~O
- A^T^A
```

- H~2~O
- A^T^A

---
### Adding keyboard keys

Keyboard keys can be rendered with a simple syntax. Consult the [Python Markdown Extensions documentation](https://facelessuser.github.io/pymdown-extensions/extensions/keys/) to learn about all available shortcodes:

```
++ctrl+alt+del++

++up+down+left+right++

++lbutton+mbutton+rbutton++
```

++ctrl+alt+del++

++up+down+left+right++

++lbutton+mbutton+rbutton++

---
## Lists

---
### Un-Ordered Lists

```
- Nulla et rhoncus turpis. Mauris ultricies elementum leo. Duis efficitur
  accumsan nibh eu mattis. Vivamus tempus velit eros, porttitor placerat nibh
  lacinia sed. Aenean in finibus diam.

    * Duis mollis est eget nibh volutpat, fermentum aliquet dui mollis.
    * Nam vulputate tincidunt fringilla.
    * Nullam dignissim ultrices urna non auctor.
```

- Nulla et rhoncus turpis. Mauris ultricies elementum leo. Duis efficitur
  accumsan nibh eu mattis. Vivamus tempus velit eros, porttitor placerat nibh
  lacinia sed. Aenean in finibus diam.

    * Duis mollis est eget nibh volutpat, fermentum aliquet dui mollis.
    * Nam vulputate tincidunt fringilla.
    * Nullam dignissim ultrices urna non auctor.

---
### Ordered Lists

```
1.  Vivamus id mi enim. Integer id turpis sapien. Ut condimentum lobortis
    sagittis. Aliquam purus tellus, faucibus eget urna at, iaculis venenatis
    nulla. Vivamus a pharetra leo.

    1.  Vivamus venenatis porttitor tortor sit amet rutrum. Pellentesque aliquet
        quam enim, eu volutpat urna rutrum a. Nam vehicula nunc mauris, a
        ultricies libero efficitur sed.

    2.  Morbi eget dapibus felis. Vivamus venenatis porttitor tortor sit amet
        rutrum. Pellentesque aliquet quam enim, eu volutpat urna rutrum a.

        1.  Mauris dictum mi lacus
        2.  Ut sit amet placerat ante
        3.  Suspendisse ac eros arcu
```

1.  Vivamus id mi enim. Integer id turpis sapien. Ut condimentum lobortis
    sagittis. Aliquam purus tellus, faucibus eget urna at, iaculis venenatis
    nulla. Vivamus a pharetra leo.

    1.  Vivamus venenatis porttitor tortor sit amet rutrum. Pellentesque aliquet
        quam enim, eu volutpat urna rutrum a. Nam vehicula nunc mauris, a
        ultricies libero efficitur sed.

    2.  Morbi eget dapibus felis. Vivamus venenatis porttitor tortor sit amet
        rutrum. Pellentesque aliquet quam enim, eu volutpat urna rutrum a.

        1.  Mauris dictum mi lacus
        2.  Ut sit amet placerat ante
        3.  Suspendisse ac eros arcu

---
### Definition Lists: 

```
`Lorem ipsum dolor sit amet`

:   Sed sagittis eleifend rutrum. Donec vitae suscipit est. Nullam tempus
    tellus non sem sollicitudin, quis rutrum leo facilisis.

`Cras arcu libero`

:   Aliquam metus eros, pretium sed nulla venenatis, faucibus auctor ex. Proin
    ut eros sed sapien ullamcorper consequat. Nunc ligula ante.

    Duis mollis est eget nibh volutpat, fermentum aliquet dui mollis.
    Nam vulputate tincidunt fringilla.
    Nullam dignissim ultrices urna non auctor.
```

`Lorem ipsum dolor sit amet`

:   Sed sagittis eleifend rutrum. Donec vitae suscipit est. Nullam tempus
    tellus non sem sollicitudin, quis rutrum leo facilisis.

`Cras arcu libero`

:   Aliquam metus eros, pretium sed nulla venenatis, faucibus auctor ex. Proin
    ut eros sed sapien ullamcorper consequat. Nunc ligula ante.

    Duis mollis est eget nibh volutpat, fermentum aliquet dui mollis.
    Nam vulputate tincidunt fringilla.
    Nullam dignissim ultrices urna non auctor.

---
### Task Lists

```
- [x] Lorem ipsum dolor sit amet, consectetur adipiscing elit
- [ ] Vestibulum convallis sit amet nisi a tincidunt
    * [x] In hac habitasse platea dictumst
    * [x] In scelerisque nibh non dolor mollis congue sed et metus
    * [ ] Praesent sed risus massa
- [ ] Aenean pretium efficitur erat, donec pharetra, ligula non scelerisque
```

- [x] Lorem ipsum dolor sit amet, consectetur adipiscing elit
- [ ] Vestibulum convallis sit amet nisi a tincidunt
    * [x] In hac habitasse platea dictumst
    * [x] In scelerisque nibh non dolor mollis congue sed et metus
    * [ ] Praesent sed risus massa
- [ ] Aenean pretium efficitur erat, donec pharetra, ligula non scelerisque

---
## Tool Tips

The Markdown syntax allows to specify a `title` for each link, which will render as a tooltip. Add a tooltip to a link with the following lines:

```title="Link Tooltip Title"
[Hover me](https://example.com "I'm a tooltip!")
```

[Hover me](https://example.com "I'm a tooltip!")

---
```title="Link Reference Tooltip"
[Hover me][example]

  [example]: https://example.com "I'm a tooltip!"
```

Tooltips can also be added to link references:

[Hover me][example]

  [example]: https://example.com "I'm a tooltip!"

---
For all other elements, a title can be added by using the Attribute Lists extension:

```
:material-information-outline:{ title="Important information" }
```

:material-information-outline:{ title="Important information" }

---
### Adding abbreviations

Abbreviations can be defined by using a special syntax similar to URLs and footnotes, starting with a `*` and immediately followed by the term or acronym to be associated in square bracket. Once an abbreviation is defined, it can be used anywhere in the document.

```title="Example Abbreviation Usage"
The HTML specification is maintained by the W3C.

*[HTML]: Hyper Text Markup Language
*[W3C]: World Wide Web Consortium
```

The HTML specification is maintained by the W3C.

*[HTML]: Hyper Text Markup Language
*[W3C]: World Wide Web Consortium

---
### Adding a glossary

```title="Example Glossary"
Lorem ipsum[^1] dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor 
incididunt ut labore et dolore magna aliqua. Ut enim[^2] ad minim veniam, quis nostrud 
exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

  [^1]:
    This is a glossary that will be added at the bottom of the page and is clickable.
  [^2]:
    This is also a glossary at the end of the page.
```
Lorem ipsum[^1] dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor 
incididunt ut labore et dolore magna aliqua. Ut enim[^2] ad minim veniam, quis nostrud 
exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

  [^1]:
    This is a glossary that will be added at the bottom of the page and is clickable.
  [^2]:
    This is also a glossary at the end of the page.
