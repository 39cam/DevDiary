# Introduction to HTML: Text-Based Elements

This section covers how to create paragraphs, headings, bold and italic text, the relationship between nested elements, and how to write HTML comments.

## Paragraphs

In HTML, paragraphs are created using the **paragraph element**.

If the browser encounters multiple line breaks in the HTML source **without** paragraph tags, it will collapse them into a single space. This causes the text to appear as one continuous line.

To properly separate text into paragraphs, we must wrap the content using the paragraph element, which automatically adds spacing after each paragraph.

```html
<p>
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
  incididunt ut labore et dolore magna aliqua.
</p>
```

## Headings

Headings are special text elements that are displayed larger and bolder to indicate section titles.

```html
<h1> to <h6>
```

HTML provides six heading levels:

Heading levels define a content hierarchy.

```html
<h1> should be used for the main title of the page.
Lower-level headings (<h2>–<h6>) should be used for subsections.
```

Using the correct heading structure improves readability, accessibility, and SEO.

## Strong Element

The strong element is used to make text bold and to semantically mark it as important.

This semantic meaning is useful for assistive technologies such as screen readers, which may change their tone to emphasize the importance of the text.

To create strong text, wrap the content with the strong tag.

```html
<strong>Important text</strong>
```

In practice, the strong element is often combined with other text elements.

## Emphasis Element

The em element is used to italicize text and to indicate emphasis.

Like the strong element, it also carries semantic meaning that can affect how assistive technologies interpret the content.

To emphasize text, wrap it with the em tag:

```html
<em>Some emphasized text</em>
```

The em element is commonly used alongside other text elements rather than on its own.

## Nesting and Indentation

HTML elements can be placed inside other elements. This is known as nesting.

When elements are nested:
* The outer element is the parent
* The inner element is the child

```html
<html>
  <head>
  </head>
  <body>
    <p>Lorem ipsum dolor sit amet.</p>
  </body>
</html>
```

In this case:
*	<body> is the parent
*   <p> is the child

Elements that share the same parent and level of nesting are called siblings.

```html
<body>
  <p>Lorem ipsum dolor sit amet.</p>
  <p>Ut enim ad minim veniam.</p>
</body>
```

Indentation helps make nesting clear and improves readability. A common convention is to indent child elements by two spaces per level.

## HTML Comments

HTML comments are not displayed in the browser. They are used to leave notes for other developers or for future reference.

Comments can provide context or explain parts of the code that may not be immediately clear.

To write an HTML comment, enclose the text between <!-- and -->.

```html
<h1>View the HTML to see the hidden comments</h1>

<!-- This is an HTML comment -->

<p>Some paragraph text</p>

<!-- Another comment -->
```

Notes
* These examples focus on readability and best practices.
* Indentation and semantic elements improve maintainability.
* Proper structure benefits accessibility and collaboration.