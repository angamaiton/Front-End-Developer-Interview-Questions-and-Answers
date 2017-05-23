# CSS Questions

#### What is the difference between classes and ID's in CSS?

*Not answered yet*

#### What's the difference between "resetting" and "normalizing" CSS? Which would you choose, and why?

Resetting removes all of the native styles provided by a given browser --
normalizing CSS makes browser styles consistent across different platforms. I
usually prefer to normalize my styles rather than reset them beforehand, as it's
less work and can help sites feel more like they belong on a device natively
(system fonts, etc.).

#### Describe Floats and how they work.

Floats are CSS properties which specify where an element should be placed within
its container -- text and other inline elements will wrap around it. Elements
can be floated left or right, or receive the property `none`.

#### Describe z-index and how stacking context is formed.

`z-index` is like the Z axis on a Cartesian plane -- it tells elements what
order to stack themselves on a screen. Stacking context is formed by a root
element and is calculated according to its children's properties (in ascending
order).

#### Describe BFC(Block Formatting Context) and how it works.

BFC is part of CSS rendering on webpages. It's used to determine how positioning
and clearing should be done. Context is created by a root element, floats,
inline-blocks, absolutely positioned elements, and/or tables.

#### What are the various clearing techniques and which is appropriate for what context?

```css
clear:both;
```

```css
overflow: hidden;
height: auto;
```

#### Explain CSS sprites, and how you would implement them on a page or site.

CSS sprites are combinations of images merged into one large image -- styling is
used to render each piece appropriately given its context (examples being
`background: url(...) x-axis y-axis;` and `background-image` alongside
`background-position`).

#### What are your favourite image replacement techniques and which do you use when?

*Not answered yet*

#### How would you approach fixing browser-specific styling issues?

*Not answered yet*

#### How do you serve your pages for feature-constrained browsers?

*Not answered yet*

###### What techniques/processes do you use?

*Not answered yet*

#### What are the different ways to visually hide content (and make it available only for screen readers)?

*Not answered yet*

#### Have you ever used a grid system, and if so, what do you prefer?

Yes. I prefer using grid systems like Lost Grid and Neat.

#### Have you used or implemented media queries or mobile specific layouts/CSS?

Yes.

#### Are you familiar with styling SVG?

I am, yes.

#### How do you optimize your webpages for print?

```css
@media print {
  ...
}
```

#### What are some of the "gotchas" for writing efficient CSS?

Usually about CSS selectors.

- Avoid key selector for large numbers of elements
- Prefer class and ID selector to tag selector
- Avoid redundant selectors
- Care of batching

#### What are the advantages/disadvantages of using CSS preprocessors?
###### Describe what you like and dislike about the CSS preprocessors you have used.



#### How would you implement a web design comp that uses non-standard fonts?

- `@font-face` to write my own `font-family`
- `@import` to import prepared web font(e.g. Google Webfonts)

#### Explain how a browser determines what elements match a CSS selector.

- Reads right-to-left
  - Check matching elements for the key(right-most) selector
  - Check if the elements are matching parents for the next selectors

#### Describe pseudo-elements and discuss what they are used for.

It's to style a part of an element, like `::first-letter` or `::before`.

They can be used to add a special symbol before a paragraph, change color of
first character of a line, etc.

#### Explain your understanding of the box model and how you would tell the browser in CSS to render your layout in different box models.

*Not answered yet*

#### What does ```* { box-sizing: border-box; }``` do? What are its advantages?

*Not answered yet*

#### List as many values for the display property that you can remember.

*Not answered yet*

#### What's the difference between inline and inline-block?

*Not answered yet*

#### What's the difference between a relative, fixed, absolute and statically positioned element?

*Not answered yet*

#### The 'C' in CSS stands for Cascading.  How is priority determined in assigning styles (a few examples)?  How can you use this system to your advantage?

#### What existing CSS frameworks have you used locally, or in production? How would you change/improve them?

I started out with Bootstrap 3, and have since switched to several different
frameworks -- Bulma, Material Design Lite, Semantic UI, and Kendo among them. I
enjoy each of them, but I think most projects deserve a tailored and smaller
framework. I usually stick to some kind of grid framework like Neat or Lost
Grid, and tailor styles to my needs.

#### Have you played around with the new CSS Flexbox or Grid specs?

Yes.

#### How is responsive design different from adaptive design?

#### Have you ever worked with retina graphics? If so, when and what techniques did you use?

```css
@media (-webkit-min-device-pixel-ratio: 1.25), (min-resolution: 120dpi) {
  ...
}
```

#### Is there any reason you'd want to use `translate()` instead of *absolute positioning*, or vice-versa? And why?

