---
layout: post
title:  "Responsive Design"
author: patrick
categories: [Responsiveness, Web]
image: assets/images/responsive.jpg
beforetoc: "Responsive Design"
toc: false
---

## Resonspive Design with Media Queries

Media Queries are a new technique introduced in CSS3 that change the presentation of content based on different viewport sizes. The viewport is a user's visible area of a web page, and is different depending on the device used to access the site.

Media Queries consist of a media type, and if that media type matches the type of device the document is displayed on, the styles are applied. You can have as many selectors and styles inside your media query as you want.

Here's an example of a media query that returns the content when the device's width is less than or equal to 100px:

```css
@media (max-width: 100px) { /* CSS Rules */ }
```

and the following media query returns the content when the device's height is more than or equal to 350px:

```css
@media (min-height: 350px) { /* CSS Rules */ }
```

Remember, the CSS inside the media query is applied only if the media type matches that of the device being used.

## Responsive Image

Making images responsive with CSS is actually very simple. You just need to add these properties to an image:

```css
img {
  max-width: 100%;
  height: auto;
}
```

The max-width of 100% will make sure the image is never wider than the container it is in, and the height of auto will make the image keep its original aspect ratio.

## Responsive Typography

Make Typography ResponsivePassed
Instead of using em or px to size text, you can use viewport units for responsive typography. Viewport units, like percentages, are relative units, but they are based off different items. Viewport units are relative to the viewport dimensions (width or height) of a device, and percentages are relative to the size of the parent container element.

The four different viewport units are:

* vw (viewport width): 10vw would be 10% of the viewport's width.
* vh (viewport height): 3vh would be 3% of the viewport's height.
* vmin (viewport minimum): 70vmin would be 70% of the viewport's smaller dimension (height or width).
* vmax (viewport maximum): 100vmax would be 100% of the viewport's bigger dimension (height or width).
Here is an example that sets a body tag to 30% of the viewport's width.

```css
body { width: 30vw; }
```
