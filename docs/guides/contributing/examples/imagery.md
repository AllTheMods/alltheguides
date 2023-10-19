# Imagery

### Resizing

Images can be done as normal,

`![](link_to_image.png)`

![](../../../assets/images/atm.png)

Images can also be clicked, but if wondering you can put captions inside `[]`

`![All The Mods Logo](link_to_image.png)`

![All The Mods Logo](../../../assets/images/atm.png)

However you can also define sizes for images, as you would with CSS.

`![](link_to_image.png){width='25px'}`

![](../../../assets/images/atm.png){width='25px'}

Within `{}` you can define your HTML tag attributes. You could even use `style`

`![](link_to_image.png){style='width: 50px'}`

![](../../../assets/images/atm.png){style='width: 50px'}

And multiple attributes at that

`![](link_to_image.png){width='75px' height='75px'}`

![](../../../assets/images/atm.png){width='75px' height='75px'}

> Note: A space cannot be between the link and `{}`.

### Images With Links

Similar to images, clicking images below would redirect you too google

`[![](link_to_image.png)](https:/google.com)`

You can also use the same attribute properties for width, height, style, etc

`[![](link_to_image.png){width='100px' height='100px'}](https:/google.com)`

[![](../../../assets/images/atm.png){width='100px' height='100px'}](https:/google.com)

### Gifs

Works the same way as images.

### Videos

`![type:video](url_to_video.mp4)`

> YouTube embed links & html iframe can also work. `https://youtube.com/embed/<VIDEO_ID>`

### Styles

As before you can use style (CSS) to add some more customizations

```
![](link_to_image.png){style='border: 3px solid red; transform: rotate(45deg); width: 125px; height: 125px'}
```

![](../../../assets/images/atm.png){style='border: 3px solid red; transform: rotate(45deg); width: 125px; height: 125px'}


