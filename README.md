# CSS

## How to add style rules to our page

1. inline
2. internal element
3. external stylesheet

## Selectors

Selectors target which elements on our page will be styled

1. Target all elements of a specific tag
2. target elements based on its attributes

- classes
- ids
- pseudo classes
- attributes
- combinators

3. elements depending are they are placed relative to others in the document

## Inheritance

Child element inherits some CSS properties from the parents in the document tree.

## Cascading StyleSheets

A particular element in the HMTL might be the target of several style declarations resulting in conflicting rules that the browser needs to resolve.

The styles in cascaded style sheets are processed by the web browser in a **certain order** that we call **the cascade:**

### Cascading Order:

I. Sort by weight and origin of the styles
II. Sort by specificity - more specific selectors will override more general ones
III. Sort by order styles are listed

### Order by weight and origin

1. !important user styles
2. !important author styles
3. Author styles

i. inline style sheets
ii. internal style sheets
iii. external style sheets

4. User styles
5. browser default styles

### II. Specificity

Each selector of a style declaration has a calculated specificty.

a= presence of an inline style
b= calculate the number of ID attributes in the selector
c= calculate the number of classes, pseudo-classes and other attributes in the selector
d= calculate the number of element names in the selector

a*100, b*10, c\*1

- has a 0 specificity

### III. Inheritance

### IV.

#### !important

Will give the priority to this rule. Not to be abused

ex.:

p {
color: red !important;
}

#quote {
color: blue;
}

<p id = "quote">This will be red</p>

References:
[When Using !important is The Right Choice](https://css-tricks.com/when-using-important-is-the-right-choice/)
[css specificity](https://www.smashingmagazine.com/2007/07/css-specificity-things-you-should-know/)
[Specifics on CSS Specificity](https://css-tricks.com/specifics-on-css-specificity/)
[CSS Selectors](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Simple_selectors)
[Users Style Sheets](https://www.viget.com/articles/inline-styles-user-style-sheets-and-accessibility/)
https://appendto.com/2016/04/css-important-rule-how-to-use-it-correctly/
