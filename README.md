# Conquering Responsive Layouts

The following are my key takeaways from [Kevin Powell](https://www.kevinpowell.co/)'s 21-day challenge of learning to create responsive layouts.

The above folders are my solutions with the given challenges. \
See and explore this repo, I'm open with any kind of feedback you have in mind.

## Day 1 - Using percentage `%` avoiding heights

#### `em` and `rem`

**Percentage vs. Fixed Widths**

- use `%` instead of `px`.
- a website is naturally responsive.

**Percentages on the child**

- Child is always dependent w/ parent interms of size.

**Avoid using `height` property**

- instead use `padding` if you want more background.

## Day 2 - Getting Familiar w/ relative units

**`em`**

- in relation w/ element's parent.

**`rem`**

- it stands for **root-`em`**.
- it will look to html font size.

**Note:** if you set `padding`, `margin`, or `border` with `em`, it looks to the `font-size` property of the parent element.

**Why you shouldn't set `font-size` using `em`?** \
**Answer:** it is compounding, font-size will get _a lot bigger_.

- use `rem` for `font-size` property.
- use `em` for `padding`, `margin`, and `border` properties.

## Day 3 - Enter `max-width`

Using `max-width` with your container limits stretching from 1 side to the other.

**CSS viewports:** \
`vh` - viewport height \
`vw` - viewport width \
`vmin` - viewport minimum \
`vmax` - viewport maximum

`%` - _Percentage_ sign, is always dependent with its parent size

**Note:** when using `vh` as height also use padding with the `vh` property to make it responsive. \
_use `vmin` for bigger font-size._

For best practice with your CSS:

```
html {
        box-sizing: border-box;
}

*, *::before, *::after {
        box-sizing: inherit;
}
/*For additional ONLY, if you want to stay the image size as it is.*/
img {
        box-sizing: content-box;
}
```

## Day 8 - Flexbox basic

**`div`** - by default has a width of 100%. \
**flex items** - by default want to be the smallest item it can be.

## Day 15 - Media Query Basics

#### Media query examples:

`@media (min-width: 600px;) {...}` \
 `min` here means `600px` or bigger. \
 this query is a mobile first approach

`@media (max-width: 600px;) {...}` \
 `max` here means `600px` or smaller. \
 this query is a desktop first approach

**Note:** Bottom `@media` query will always rule your code.
