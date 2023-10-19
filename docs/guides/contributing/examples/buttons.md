# Buttons

Material for MkDocs provides dedicated styles for primary and secondary buttons that can be added to any link, `label` or `button` element. This is especially useful for documents or landing pages with dedicated call-to-actions.

### Buttons

In order to render a link as a button, suffix it with curly braces and add the .md-button class selector to it.

`[Subscribe to our newsletter](#){ .md-button }`

[Subscribe to our newsletter](#){ .md-button }

### Adding primary buttons¶

If you want to display a filled, primary button (like on the landing page of Material for MkDocs), add both, the .md-button and .md-button--primary CSS class selectors.

`[Subscribe to our newsletter](#){ .md-button .md-button--primary }`

[Subscribe to our newsletter](#){ .md-button .md-button--primary }

### Adding icon buttons¶

Of course, icons can be added to all types of buttons by using the [icon syntax](https://squidfunk.github.io/mkdocs-material/reference/icons-emojis/#using-icons) together with any valid icon shortcode, which can be easily found with a few keystrokes through [icon search](https://squidfunk.github.io/mkdocs-material/reference/icons-emojis/#search).

`[Send :fontawesome-solid-paper-plane:](#){ .md-button }`

[Send :fontawesome-solid-paper-plane:](#){ .md-button }