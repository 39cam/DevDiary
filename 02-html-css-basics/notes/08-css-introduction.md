# CSS: Introduction  

## What is CSS?  

Before anything else, it’s important to understand that a web page is essentially a text document. In this document you write all your HTML code, which defines the structure and content of the page.  

CSS is a separate language that works alongside HTML. While HTML defines *what* is on the page, CSS is responsible for how it looks — including colors, layout, spacing, positioning, and overall visual style.  

## What does CSS mean?  

CSS stands for **Cascading Style Sheets**. The idea behind it is simple but very powerful: apply visual styles (such as colors, shapes, margins, and spacing) to one or multiple documents — usually HTML files — in an automatic and consistent way.  

A common approach is to have many HTML files but only one CSS file. Each HTML document links to this single stylesheet. This way, if you make a change in the CSS file, it will automatically affect all the connected web pages.  

## Why is CSS used?  

CSS allows us to separate content from presentation. This makes websites much easier to maintain and update over time.  

Instead of changing styles in every single HTML file, you can modify them in one central CSS file and have those changes reflected across the entire site. This also reduces repetition and keeps your code cleaner and more organized.  

## Basic syntax  

At its core, CSS consists of rules. Each rule contains:  
- A **selector**, which targets the HTML element you want to style.  
- One or more **declarations**, each made up of a property and a value.  

Example:  

```css
div.bold-text { /* selector */
    font-weight: 700; /* property: value */
}