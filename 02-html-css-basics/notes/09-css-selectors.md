# CSS: Selectors

## Selector

Selector refer to the hTML element to which CSS rules apply; they're what is actually being "selected" for each rule. 

## Universal selector

The universal selector will select elements of every type (as in the whole document), hence the name "universal", and the syntax for it is a simple asterisk. In the example below, every element would have the color: purple; style applied it

```css
* {
  color: purple;
}
```

## Type selector

A type selector (or element selector) will select all elements of the given element type, and the syntax is just the name of the element:

```html
<!-- index.html -->

<div>Hello, World!</div>
<div>Hello again!</div>
<p>Hi...</p>
<div>Okay, bye.</div>
```

```css
/* styles.css */

div {
  color: white;
}
```

Here, all three <div> elements would be selected, while the <p> element wouldn't be

## Class selectors 

Class selectors will select all elements with the given class, which is just an attribute you place on an HTML element.

```html
<div class="alert-text">Please agree to our terms of service.</div>

```

```css
.alert-text {
  color: red;
}
```

Syntax for class selectors: a period inmediately followed by the case-sensitive value of the class attrubute. Classes aren't required to be specific to a particular element, so you can use the same class on as many elements as you want.

Class selectors won't work if the class name begins with a number, like 1-element, using a .1-elements as a selector won't match it.

You can add multiple classes to a single element as a space-separated list, such as class="alert-text severe-alert". Since whitespace is sed to separate class names like this, you should never use spaces for multi-worded names and should use a hyphen instead.

## ID selectors

ID selectors are similar to class selectors. The select an element with the given ID, which is another attribute you place on an HTML elements. The major difference between classes and IDs is that an element can only have one ID. It cannot be repeated on a single page and should noy contain any whitespace:

```html
<div id='tittle">My page</div>
```

```css
#tittle{
  background-color: red;
}
```

For IDs, instead of a period, we use a hashtag in