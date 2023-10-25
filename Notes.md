# [Introduction](https://www.w3schools.com/html/html_intro.asp)

## Tags
- `<!DOCTYPE html>` defines that the document is a HTML5 document
- `<html>` is the root element of a HTML page
- `<head>` contains meta information of a HTML page
- `<title>` specifies a title for the HTML page (which is shown in the browser's title bar or in the page's tab)
- `<body>`  defines the document's body, and is a container for all the visible contents, such as headings, paragraphs, images, hyperlinks, tables, lists, etc.
- `<h1>` defines a large heading
- `<p>` defines a paragraph

## HTML
- Stands for Hyper Text Markup Language
- Standard markup for creating web pages
- Describes structure of a web page
- Consists of series of elements
- Tells the browser how to display the content

# [Basic Examples](https://www.w3schools.com/html/html_basic.asp)

## HTML documents
- Must start with `<!DOCTYPE HTML>`
- Begins with `<html>` and ends with `</html>`
- Visible part begins with `<body>` and ends with `</body>`

## The `<!DOCTYPE>` declaration
- Represents the document type
- Helps browsers display web pages correctly
- Must only appear once
- Only at the top of the page (before any HTML tags)
- Not case sensitive
- Defined with the `<!DOCTYPE html>` tag

## HTML Headings
- Defined with the `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>` & `<h6>` tags
- `<h1>` defines the most important
- `<h6>` defines the least important

## HTML paragraphs
- Defined with the `<p>` tag

## HTML Links
- Defined with the `<a>` tag
- Destination is specified in the `href` attribute

## HTML Images
- Defined with the `<img>` tag
- Source file is in the `src` attribute
- Alternative text is in the `alt` attribute
- `width` and `height` are also attributes

# [Elements](https://www.w3schools.com/html/html_elements.asp)
## What is a HTML element?
- Everything from a start tag, content and an end tag
```html
<tag>content</tag>
```
- Can be nested (Elements can contain other elements)
- All HTML documents consist of nested HTML elements
- Some HTML documents will display correctly, even if the end tag is missing (**Never rely on this; Unexpected results and errors may occur if you leave out the end tag**)
- Some HTML elements have no content
- They are known as empty elements
- Empty elements have no end tags
- For example, the `<br>` tag defines a line break
- HTML tags are not case sensitive
- `<P>` is the same as `<p>`
- The HTML standard does not require lowercase tags
- World Wide Web Consortium **recommends** lowercase in HTML, and **demands** lowercase for stricter document types like XHTML