# Code

``````
``` py
import tensorflow as tf
```
``````

``` py
import tensorflow as tf
```

### Adding Titles

In order to provide additional context, a custom title can be added to a code block by using the `title="<custom title>"` option directly after the shortcode, e.g. to display the name of a file:

``````
``` py title="bubble_sort.py"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```
``````

``` py title="bubble_sort.py"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```

### Adding annotations

Code annotations can be placed anywhere in a code block where a comment for the language of the block can be placed, e.g. for JavaScript in `// ...` and `/* ... */`, for YAML in `# ...`, etc.

``````
``` yaml
theme:
  features:
    - content.code.annotate # (1)
```

1.  :man_raising_hand: I'm a code annotation! I can contain `code`, __formatted
    text__, images, ... basically anything that can be written in Markdown.
``````

``` yaml
theme:
  features:
    - content.code.annotate # (1)
```

1.  :man_raising_hand: I'm a code annotation! I can contain `code`, __formatted
    text__, images, ... basically anything that can be written in Markdown.


### Stripping comments

If you wish to strip the comment characters surrounding a code annotation, simply add an `!` after the closing parenthesis of the code annotation:

``````
``` yaml
# (1)!
```

1.  Look ma, less line noise!
``````

``` yaml
# (1)!
```

1.  Look ma, less line noise!

### Adding line numbers

Line numbers can be added to a code block by using the `linenums="<start>"` option directly after the shortcode, whereas `<start>` represents the starting line number. A code block can start from a line number other than `1`, which allows to split large code blocks for readability:

``````
``` py linenums="1"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```
``````

``` py linenums="1"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```

#### Highlighting specific lines

Specific lines can be highlighted by passing the line numbers to the `hl_lines` argument placed right after the language shortcode. Note that line counts start at `1`, regardless of the starting line number specified as part of `linenums`:

``````
``` py hl_lines="2 3"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```
``````

``` py hl_lines="2 3"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```

### Highlighting inline code blocks

Syntax highlighting can be applied to inline code blocks by prefixing them with a shebang, i.e. #!, directly followed by the corresponding `language shortcode`.

```
The `#!python range()` function is used to generate a sequence of numbers.
```

The `#!python range()` function is used to generate a sequence of numbers.
