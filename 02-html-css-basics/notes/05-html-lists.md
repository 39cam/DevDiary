# Introduction to HTML: Lists

HTML lists are used to group related items together in a structured way. They help organize content and improve readability on a webpage.

---

## Unordered Lists

An **unordered list** is used when the order of the items does not matter. A common example is a shopping list, where items can appear in any sequence.

Unordered lists are created using the `ul` element, and each item inside the list is defined with the `li` element. By default, each item is displayed with a bullet point.

Example:

```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>
```

---

## Ordered Lists

An ordered list is used when the order of items is important, such as step-by-step instructions or ranked lists.

Ordered lists are created using the ol element. Like unordered lists, each item is defined using the li element. The difference is that items are automatically numbered.

```html
<ol>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ol>
```

---

## Description Lists

A description list is used to pair terms with their corresponding descriptions.

This type of list uses:
*	dl to define the list
*	dt to define the term
*	dd to define the description of the term

```html
<dl>
  <dt>Coffee</dt>
  <dd>Black hot drink</dd>

  <dt>Milk</dt>
  <dd>White cold drink</dd>
</dl>
```

## Common List Tags Summary

| Tag | Description |
|-----|-------------|
| `ul` | Defines an unordered list |
| `ol` | Defines an ordered list |
| `li` | Defines a list item |
| `dl` | Defines a description list |
| `dt` | Defines a term in a description list |
| `dd` | Defines the description of a term |