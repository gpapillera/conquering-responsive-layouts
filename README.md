# Conquering Responsive Layouts

The following are my key takeaways from [Kevin Powell](https://www.kevinpowell.co/)'s 21-day challenge of learning to create responsive layouts.

## Day 1 - Using percentage % avoiding heights
#### `em` and `rem`

**Percentage vs. Fixed Widths**
- use `%` instead of `px`.
- a website is naturally responsive. \
**Percentages on the child**
- Child is always dependent w/ parent interms of size. \
**Avoid using `height` property**
- instead use `padding` if you want more background.

## Day 2 - Getting Familiar w/ relative units

**`em`**
- in relation w/ element's parent. \
**`rem`**
- it stands for root-`em`.
- it will look to html font size.

**Note:** if you set padding, margin, or boder with `em`, it looks to the `font-size` property of the parent element.
