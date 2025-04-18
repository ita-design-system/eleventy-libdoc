---
layout: libdoc_page.liquid
eleventyNavigation:
    key: Images widgets
    parent: Widgets
description: Ready to use HTML to highlight your images
permalink: creating-content/widgets/images/index.html
---

[Markdown images](/content/creating-content/markdown.md#images) are useful for everyday use but sometime it comes you have to highlight your images.

## Light background on images with transparency

`light` class name on `<img>` tag applies a white background on image.

<img class="light"
    src="/assets/images/gypaetus-barbatus-peisey.png"
    alt="Gypaetus barbatus">

```html
<img class="light"
    src="/assets/images/gypaetus-barbatus-peisey.png"
    alt="Gypaetus barbatus">
```

## Dark background on images with transparency

`dark` class name on `<img>` tag applies a black background on image.

<img class="dark"
    src="/assets/images/gypaetus-barbatus-peisey.png"
    alt="Gypaetus barbatus">

```html
<img class="dark"
    src="/assets/images/gypaetus-barbatus-peisey.png"
    alt="Gypaetus barbatus">
```

## Damier background to images with transparency

`damier` class name on `<img>` tag highlights transparency.

<img class="damier"
    src="/assets/images/gypaetus-barbatus-peisey.png"
    alt="Gypaetus barbatus">

```html
<img class="damier"
    src="/assets/images/gypaetus-barbatus-peisey.png"
    alt="Gypaetus barbatus">
```

## Rounded corners

`rounded-corners` class name on `<img>` tag allows to apply smooth corners on the image.

<img class="rounded-corners"
    src="/assets/images/pierra-menta.jpg"
    alt="Pierra Menta">

```html
<img class="rounded-corners"
    src="/assets/images/pierra-menta.jpg"
    alt="Pierra Menta">
```

## Long shadow

`long-shadow` class name on `<img>` tag allows to apply a long box shadow.

<img class="long-shadow"
    src="/assets/images/pierra-menta.jpg"
    alt="Pierra Menta">

```html
<img class="long-shadow"
    src="/assets/images/pierra-menta.jpg"
    alt="Pierra Menta">
```

## Filter long shadow

`filter-long-shadow` class name on `<img>` tag allows to apply drop shadow on non-transparent pixels.

<img class="filter-long-shadow"
    src="/assets/images/gypaetus-barbatus-peisey.png"
    alt="Gypaetus barbatus">

```html
<img class="filter-long-shadow"
    src="/assets/images/gypaetus-barbatus-peisey.png"
    alt="Gypaetus barbatus">
```

## Boxed image

Boxed images require specific markup as follows but keeps same features class names as previously.

<figure>
    <img src="/assets/images/pierra-menta.jpg" alt="Pierra Menta">
    <figcaption>A basic boxed image with its long description.</figcaption>
</figure>

```html
<figure>
    <img src="/assets/images/pierra-menta.jpg" alt="Pierra Menta">
    <figcaption>A basic boxed image with its long description.</figcaption>
</figure>
```

## Boxed image wide

The `wide` class name allows to feature an image.

<figure class="wide">
    <img src="/assets/images/pierra-menta.jpg"
        alt="Pierra Menta"
        eleventy:widths="1400,2800">
    <figcaption>
        A wide boxed image with its description.
        Class name applied on figure:
        <code>wide</code>.
    </figcaption>
</figure>

```html
<figure class="wide">
    <img src="/assets/images/pierra-menta.jpg"
        alt="Pierra Menta"
        eleventy:widths="1400,2800">
    <figcaption>
        A wide boxed image with its description.
        Class name applied on figure:
        <code>wide</code>.
    </figcaption>
</figure>
```

## Mixed features

`rounded-corners` and `long-shadow`.

<img class="rounded-corners long-shadow"
    src="/assets/images/pierra-menta.jpg"
    alt="Pierra Menta">

```html
<img class="rounded-corners long-shadow"
    src="/assets/images/pierra-menta.jpg"
    alt="Pierra Menta">
```

<figure class="rounded-corners long-shadow wide">
    <img src="/assets/images/pierra-menta.jpg"
        alt="Pierra Menta"
        eleventy:widths="1400,2800">
    <figcaption>
        A wide boxed image with rounded corners and a long box shadow, with its long description.
        Class names applied on figure:
        <code>rounded-corners</code>,
        <code>long-shadow</code> and 
        <code>wide</code>.
    </figcaption>
</figure>

```html
<figure class="rounded-corners long-shadow wide">
    <img src="/assets/images/pierra-menta.jpg"
        alt="Pierra Menta"
        eleventy:widths="1400,2800">
    <figcaption>
        A wide boxed image with rounded corners and a long box shadow, with its long description.
        Class names applied on figure:
        <code>rounded-corners</code>,
        <code>long-shadow</code> and 
        <code>wide</code>.
    </figcaption>
</figure>
```

<figure class="wide">
    <img src="/assets/images/gypaetus-barbatus-peisey.png"
        alt="Gypaetus barbatus"
        eleventy:widths="1400,2800">
    <figcaption>
        A wide boxed image with its long description.
        Class name applied on figure: 
        <code>wide</code>.
    </figcaption>
</figure>

```html
<figure class="wide">
    <img src="/assets/images/gypaetus-barbatus-peisey.png"
        alt="Gypaetus barbatus"
        eleventy:widths="1400,2800">
    <figcaption>
        A wide boxed image with its long description.
        Class name applied on figure: 
        <code>wide</code>.
    </figcaption>
</figure>
```

<figure class="filter-long-shadow wide">
    <img src="/assets/images/gypaetus-barbatus-peisey.png"
        alt="Gypaetus barbatus"
        eleventy:widths="1400,2800">
    <figcaption>
        A wide boxed image with filter drop shadow, with its long description.
        Class names applied on figure: 
        <code>filter-long-shadow</code> and <code>wide</code>.
    </figcaption>
</figure>

```html
<figure class="filter-long-shadow wide">
    <img src="/assets/images/gypaetus-barbatus-peisey.png"
        alt="Gypaetus barbatus"
        eleventy:widths="1400,2800">
    <figcaption>
        A wide boxed image with filter drop shadow, with its long description.
        Class names applied on figure: 
        <code>filter-long-shadow</code> and <code>wide</code>.
    </figcaption>
</figure>
```


