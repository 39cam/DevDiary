# Introduction to HTML: Links and Images

Links are one of the most important features of HTML. They make it possible to connect different pages across the internet, which is why this system is known as the *Web*.

---

## Anchor elements

To create a link in HTML, we use the **anchor element**. This is done by wrapping the text (or another element) that we want to turn into a link inside an `<a>` tag.

```html
<a>About this repository</a>
```

If you click this link, nothing will happen. This is because an anchor tag by itself does not specify where the link should go. We need to provide a destination using an **HTML attribute**.

An HTML attribute adds extra information to an element and is always placed inside the opening tag. Attributes usually consist of a name and a value.

To define where a link should point, we use the **href (hypertext reference)** attribute. Its value is the URL of the destination.

```html
<a href="https://www.youtube.com/watch?v=aUMB5lzBI2s">About this repository</a>
```

By default:
* An anchor without href looks like normal text.
* An anchor with href appears blue and underlined, indicating that it is clickable.

Anchor tags can link to many types of resources, such as:
* Other webpages
* Videos
* PDF files
* Images

However, most of the time they are used to link to other HTML documents.

## Opening links in a new tab

By default, links open in the same tab as the current page. This behavior can be changed using the target attribute.
* target="_self" → Opens in the same tab (default)
* target="_blank" → Opens in a new tab or window

Example:

``html
<a href="https://www.youtube.com/watch?v=aUMB5lzBI2s" target="_blank" rel="noreferrer">
  About this repository
</a>
``

### About the rel attribute

The rel attribute describes the relationship between the current page and the linked page. Two common values are:
* noopener: Prevents the new tab from accessing the original page, reducing security risks such as tabnabbing. Modern browsers apply this automatically when using target="_blank".
* noreferrer: Does the same as noopener, but also hides referral information from the destination page.

## Absolute and relative links

There are two main types of links in HTML:

**Absolute links**

These point to pages on external websites and always include the full web address in the format:

``code
scheme://domain/path
``

Example of an absolute link:

``code
[scheme://domain/path](https://www.youtube.com/@Pablohzdev)
``

This includes both the protocol and the domain.

## Relative links

These point to pages within the same website and do not include the domain name.

Instead, they specify the path to another file relative to the current page.

For example, inside a folder named project-images/, you could create a file called about.html containing:

```html
<h1>Homepage</h1>
```

A relative link from another file in the same folder could be:

```html
<a href="./about.html">Go to homepage</a>
```

Since both files are in the same directory, no full URL is needed.

if they're in different directories we need to change it using ./

## Images

Web pages would be quite limited if they could only show text. Fortunately, HTML includes several elements that allow us to display different types of media, with the most common being the image element.

To insert an image into an HTML document, we use the `<img>` element. Unlike most other elements, `<img>` is a **void element**, meaning it does not have a closing tag because it does not wrap any content.

Instead of containing text, the image element uses a `src` (source) attribute to specify the location of the image file. This works in a similar way to the `href` attribute in anchor tags and can reference images using either absolute or relative paths.

For example, an image hosted on an external website can be embedded using an absolute URL:

```html
<img src="https://yt3.googleusercontent.com/E4lvXbL82lxD-KO-lpoHxvOAWVXTfKEHQhUYl0suFHmVFLj2p-54Hht92BdSvsyZnsfDql7uSg=s160-c-k-c0x00ffffff-no-rj">
```

If the image is stored on your own server, you can instead use a relative path.

---

## Parent directories

If we want to display an image that is located in a different folder, we may need to move up to a parent directory before accessing it.

To move up one level in a file path, we use `../`. This tells the browser to go to the parent directory of the current file.

For example, inside `about.html`, you could include an image like this:

```html
<img src="../images/example.jpg">
```

Breaking this down:
- `../` moves up from the current folder to its parent directory.
- `images/` enters the images folder.
- `example.jpg` is the actual image file being loaded.

You can think of `../` like stepping out of your current room into a hallway so you can enter another room.

---

## Alt attribute

Every image should include an `alt` (alternative text) attribute in addition to `src`.

The `alt` attribute provides a textual description of the image. It is used:
- If the image fails to load
- By screen readers to describe images to visually impaired users
- By search engines to understand image content

Example with an alt attribute:

```html
<img src="https://yt3.googleusercontent.com/E4lvXbL82lxD-KO-lpoHxvOAWVXTfKEHQhUYl0suFHmVFLj2p-54Hht92BdSvsyZnsfDql7uSg=s160-c-k-c0x00ffffff-no-rj"alt="Profile picture of Pablohzdev">
```

---

## Image size attributes

Although not strictly required, it is good practice to include `height` and `width` attributes in image tags.

Specifying these values helps the browser reserve space for the image before it loads, preventing layout shifts and content jumping.

Even if you plan to resize the image later with CSS, you should still include the original dimensions.

Example including size attributes:

```html
<img src="https://yt3.googleusercontent.com/E4lvXbL82lxD-KO-lpoHxvOAWVXTfKEHQhUYl0suFHmVFLj2p-54Hht92BdSvsyZnsfDql7uSg=s160-c-k-c0x00ffffff-no-rj" alt="Profile picture of Pablohzdev" height="310" width="310">
```