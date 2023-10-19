# Annotations

One of the flagship features of Material for MkDocs is the ability to inject annotations – little markers that can be added almost anywhere in a document and expand a tooltip containing arbitrary Markdown on click or keyboard focus.

### Using Annotations

Annotations consist of two parts: a marker, which can be placed anywhere in a block marked with the `annotate` class, and content located in a list below the block containing the marker:

```
Lorem ipsum dolor sit amet, (1) consectetur adipiscing elit.
{ .annotate }

1.  :man_raising_hand: I'm an annotation! I can contain `code`, __formatted
    text__, images, ... basically anything that can be expressed in Markdown.
```

Lorem ipsum dolor sit amet, (1) consectetur adipiscing elit.
{ .annotate }

1.  :man_raising_hand: I'm an annotation! I can contain `code`, __formatted
    text__, images, ... basically anything that can be expressed in Markdown.

> Note that the `annotate` class must only be added to the outermost block. All nested elements can use the same list to define annotations, except when annotations are nested themselves.

#### In SuperFetch

Annotations can also be nested inside annotations by adding the `annotate` class to the list item hosting the annotation content, repeating the process:

```
Lorem ipsum dolor sit amet, (1) consectetur adipiscing elit.
{ .annotate }

1.  :man_raising_hand: I'm an annotation! (1)
    { .annotate }

    1.  :woman_raising_hand: I'm an annotation as well!
```

Lorem ipsum dolor sit amet, (1) consectetur adipiscing elit.
{ .annotate }

1.  :man_raising_hand: I'm an annotation! (1)
    { .annotate }

    1.  :woman_raising_hand: I'm an annotation as well!

#### In Admonitions

The titles and bodies of [admonitions](admonition.md) can also host annotations by adding the annotate modifier after the type qualifier, which is similar to how [inline blocks](admonition.md#inline-blocks) work:

```
!!! note annotate "Phasellus posuere in sem ut cursus (1)"

    Lorem ipsum dolor sit amet, (2) consectetur adipiscing elit. Nulla et
    euismod nulla. Curabitur feugiat, tortor non consequat finibus, justo
    purus auctor massa, nec semper lorem quam in massa.

1.  :man_raising_hand: I'm an annotation!
2.  :woman_raising_hand: I'm an annotation as well!
```

#### In Content Tabs

Content tabs can host annotations by adding the `annotate` class to the block of a dedicated content tab (and not to the container, which is not supported):

```
=== "Tab 1"

    Lorem ipsum dolor sit amet, (1) consectetur adipiscing elit.
    { .annotate }

    1.  :man_raising_hand: I'm an annotation!

=== "Tab 2"

    Phasellus posuere in sem ut cursus (1)
    { .annotate }

    1.  :woman_raising_hand: I'm an annotation as well!
```

=== "Tab 1"

    Lorem ipsum dolor sit amet, (1) consectetur adipiscing elit.
    { .annotate }

    1.  :man_raising_hand: I'm an annotation!

=== "Tab 2"

    Phasellus posuere in sem ut cursus (1)
    { .annotate }

    1.  :woman_raising_hand: I'm an annotation as well!

#### In Everything Else

Tt's always possible to leverage the Markdown in HTML extension to wrap arbitrary elements with a div with the annotate class:

```
<div class="annotate" markdown>

> Lorem ipsum dolor sit amet, (1) consectetur adipiscing elit.

</div>

1.  :man_raising_hand: I'm an annotation!
```

<div class="annotate" markdown>

> Lorem ipsum dolor sit amet, (1) consectetur adipiscing elit.

</div>

1.  :man_raising_hand: I'm an annotation!

With this trick, annotations can also be added to blockquotes, lists, and many other elements that are not supported by the [Attribute Lists](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown/#attribute-lists) extension. Furthermore, note that [code blocks follow different semantics](https://squidfunk.github.io/mkdocs-material/reference/code-blocks/#adding-annotations).