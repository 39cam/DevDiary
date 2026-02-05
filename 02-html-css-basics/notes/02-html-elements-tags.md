# Introduction to HTML: How It Works

HTML (HyperText Markup Language) is the language used to define the structure and content of webpages. By using HTML elements, we can create paragraphs, headings, lists, images, and links that together form a complete webpage.

## HTML Tags

Most content on an HTML page is created by wrapping text or media inside **opening and closing HTML tags**.

HTML tags act as the core components that describe both the structure and purpose of webpage content. 

### Opening Tags

An opening tag tells the browser where an element begins. It consists of a keyword placed inside angle brackets (`<>`).

Example of an opening paragraph tag:

```html
<p>
```

### Closing Tags

Closing tags indicate the end of an element. They are similar to opening tags, but include a forward slash (`/`) before the tag name.

Example of a closing paragraph tag:

```html
</p>
```

## Example of an HTML Element

A complete paragraph element is written as follows:

```html
<p>Some text content</p>
```

Where:

	•	</p> marks the beginning of the paragraph
	•	Some text content is the content inside the element
	•	</p> marks the end of the paragraph

## HTML Elements Explained

HTML elements can be seen as **containers** that hold content. The browser reads the opening and closing tags to understand what type of content is inside and how it should be displayed.

HTML provides a large collection of predefined tags that allow developers to create many different kinds of elements. Choosing the appropriate tag for each type of content is important.

Using the correct tags affects:

- How search engines interpret and rank a website
- How accessible the site is for users who rely on assistive technologies such as screen readers

The practice of using meaningful and appropriate tags is known as **semantic HTML**.


## Void Elements

Some HTML elements do not require a closing tag. These elements consist of a single tag, such as:

```html
<br>
<img>
```

These are called **void elements**, meaning they do not contain any inner content. Because of this, they cannot wrap text or other elements.


## Self-Closing Tags

Void elements may also appear written as self-closing tags, for example:

```html
<br />
<img />
```

This syntax exists mainly for historical reasons. While modern browsers can still render these elements correctly, the current HTML specification discourages this format.

### Recommendation

For modern HTML, it is recommended to write void elements **without** the trailing slash.