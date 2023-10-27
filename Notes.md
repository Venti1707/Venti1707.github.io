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
- World Wide Web Consortium **recommends** lowercase in HTML and **demands** lowercase for stricter document types like XHTML
- For a list of HTML tags, visit this [page](https://www.w3schools.com/tags/default.asp)

# [Attributes](https://www.w3schools.com/html/html_attributes.asp)

## The `href` attribute
- The `<a>` tag defines a hyperlink
- The `href` attribute specifies the URL of the page to link to

## The `src` attribute
- The `<img>` tag is used to embed an image in a HTML page
- The `src` attribute specifies the path to the image to be displayed
- Can be specified in 2 ways
  - **Absolute URL**
    - Links to an external image that is hosted on another website
      - Example: https://raw.githubusercontent.com/Venti1707/Genshin-TCG-Assets/main/My-Cards/img/Character%20Cards/Venti.png
    - External images might be under copyright.
      - If you do not get permission to use it, you may be in violation of copyright laws.
    - Cannot control external images
      - It can suddenly be removed or changed.
  - **Relative URL**
    - Links to an image hosted within the website
    - URL does not include domain name
    - If the URL does not begin with a slash, it will be relative to the current page
      - `src="Venti.png"`
    - If the URL does begin with a slash, it will be relative to the domain
      - `src="/img/Character%20Cards/Venti.png"`
- It is better to use Relative URLs as they will not break if your domain changes

## The `width` and `height` attributes
- The `<img>` tag should also contain these
- They specify the width and height of the image in pixels

## The `alt` attribute
- Used in the `<img>`
- Specifies an alternate text for an image if the image cannot be displayed
- Reasons for the image being unable to be displayed include:
  - Slow connections
  - An error in the `src` attribute
  - If the user is using a screen reader

## The `style` attribute
- Used to add styles to an element
- Some styles include
  - Colour
  - Font
  - Size

## The `lang` attribute
- Should be included in the `<html>` tag
- This specifies English as the language
```html
<!DOCTYPE html>
<html lang="en">
  <body>
      ...
  </body>
</html>
```
- Used to declare the language of the webpage
- Meant to assist
  - Search engines
  - Browsers
- Country codes can also be added
  - First 2 characters define the language
  - Last 2 characters define the country
- This specifies English as the language and United States as the country
```html
<!DOCTYPE html>
<html lang="en-US">
  <body>
   ...
  </body>
</html>
```
- All language codes can be viewed [here](https://www.w3schools.com/tags/ref_language_codes.asp)

## The `title` attribute
- Defines extra information about an element
- Value will be displayed as a tooltip when the mouse is over the element

## Attribute Names
- HTML standard does not require lowercase attribute names
- All attributes can be written in lowercase or uppercase
- World Wide Web Consortium **recommends** lowercase in HTML and **demands** lowercase for stricter document types like XHTML

## Attribute Values
- HTML standard does not require quotes around attribute values
- World Wide Web Consortium **recommends** quotes in HTML and **demands** quotes for stricter document types like XHTML

- Good:
```html
<a href="introduction.html">Visit the introduction page!</a>
```
- Bad:
```html
<a href=introduction.html>Visit the introduction page!</a>
```
- Quotes have to be used when the attribute value contains a space
```html
<p title=About Me>
```

## Single or Double Quotes?
- Double quotes around attribute values are the most common
- Single quotes can also be used
- If the attribute value contains double quotes, then it is necessary to use single quotes and vice versa
```html
<p title="I am a title with 'single quotes'">
<p title='I am a title with "double quotes"'>
```

# [Headings](https://www.w3schools.com/html/html_headings.asp)
- Each heading has a default size
- You can specify the size for any heading with the style attribute, using the CSS `font-size` property
- Browsers automatically add some white space (also known as a margin) before and after a heading

# [Paragraphs](https://www.w3schools.com/html/html_paragraphs.asp)
- Always starts on a new line
- Browsers automatically add a margin before and after a paragraph

## Display
- You cannot be sure how HTML will be displayed
- Large, small screens and resized windows will produce different results
- With HTML, you cannot change the display by adding extra spaces or extra lines in the source code
- The browser will automatically remove any extra spaces and lines when the page is displayed

## Horizontal Rules
- Produced with the `<hr>` tag
- Defines a thematic break
- Is used to separate content (or define a change) in a HTML page
- Is an empty tag

## Line Breaks
- Produced with the `<br>` tag
- Defines a line break
- Used if a line break is needed without a new paragraph being started

## The `<pre>` Element
- Defines preformatted text
- Text inside is displayed in a fixed-width font (usually Corrier)
- Preserves
  - Spaces
  - Line breaks 

# [Styles](https://www.w3schools.com/html/html_styles.asp)

## The `style` attribute
- Used to add styles to an element
- Includes things like
  - Colour
  - Font
  - Size
  - And more
- Has the following syntax
```html
<tagname style="property: value;">
```
- `property` is a CSS property
- `value` is a CSS value

## Background Colour
- The CSS `background-color` property defines the background colour for a HTML element
- Example:
```html
<h1 style="background-color: #42BC9C;">This is a heading with the background-color style and it has a value of #42BC9C</h1>
```


## Text Colour
- The CSS `color` property defines the text colour for a HTML element
- Example:
```html
<h1 style="color: #7042DB;">This is a heading with the color style and it has a value of #7042DB</h1>
```

## Font Family
- The CSS `font-family` property defines the font to be used for a HTML element
- Example:
```html
<h1 style="font-family: verdana;">This is a heading with the font-family style and it has a value of verdana</h1>
```

## Text Size
- The CSS `font-size` property defines the text size for a HTML element
- Example:
```html
<h1 style="font-size: 300%;">This is a heading with the font-size style and it has a value of 300%</h1>
```

## Text Alignment
- The CSS `text-align` property defines the **horizontal** text alignment
- Example:
```html
<h1 style="text-align: center;">This is a heading with the text-align style and it has a value of center</h1>
```