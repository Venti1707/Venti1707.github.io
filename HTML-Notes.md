# [Introduction](https://www.w3schools.com/html/html_intro.asp)

## Tags
- `<!DOCTYPE html>` defines that the document is a HTML5 document
- `<html>` is the root element of a HTML page
- `<head>` contains meta information of a HTML page
- `<title>` specifies a title for the HTML page (which is shown in the browser's title bar or in the page's tab)
- `<body>` defines the document's body, and is a container for all the visible contents, such as headings, paragraphs, images, hyperlinks, tables, lists, etc.
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
- Used to declare the language of the web page
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

# Text Formatting

## Formatting Elements
- Designed to display special types of text
- `<b>` - Bold text
- `<strong>` - Important text
- `<i>` - Italic text
- `<em>` - Emphasized text
- `<mark>` - Marked text
- `<small>` - Smaller text
- `<del>` - Deleted text
- `<ins>` - Inserted text
- `<sub>` - Subscript text
- `<sup>` - Superscript text

## `<b>`
- Defines bold text, without any extra importance
- Example:
```html
<b>This text is bold</b>
```
## `<strong>`
- Defines text with strong importance
- Content inside is typically displayed in bold
- Example:
```html
<strong>This text is important</strong>
```

## `<i>`
- Defines part of a text in an alternate voice or mood
- Content inside is typically displayed in italic
- Used to indicate a technical term, a phrase from another language, a thought, a ship name, etc.
- Example:
```html
<i>This text is italic</i>
```

## `<em>`
- Content inside is typically displayed in italic
- Screen readers will pronounce words in `<em>` with an emphasis, using verbal stress
- Example:
```html
<em>This text is emphasized</em>
```

## `<small>`
- Defines smaller text
- Example:
```html
<small>This is some smaller text.</small>
```

## `<mark>`
- Defines text that should be marked/highlighted
- Example:
```html
<mark>This is some marked text.</mark>
```

## `<del>`
- Defines text that has been been deleted from a document
- Browsers usually strike a line through deleted text
- Example:
```html
<del>This is some deleted text.</del>
```

## `<ins>`
- Defines text that has been been inserted from a document
- Browsers usually underline inserted text
- Example:
```html
<ins>This is some inserted text.</ins>
```

## `<sub>`
- Defines subscript text
- Appears half a character below the normal line
- Sometimes rendered in a smaller font
- Can be used for chemical formulas, like C₁₂H₂₂O₁₁
- Example:
```html
<sub>This is some subscript text.</sub>
```

## `<sup>`
- Defines superscript text
- Appears half a character above the normal line
- Sometimes rendered in a smaller font
- Can be used for footnotes, like <sup>[1]</sup>
- Example:
```html
<sup>This is some superscript text.</sup>
```

# [Quotation and Citation](https://www.w3schools.com/html/html_quotation_elements.asp)

## `<blockquote>`
- Defines a section that is quoted from another source
- Browsers usually indent `<blockquote>` elements
- Example:
```html
<blockquote cite="https://www.youtube.com/watch?v=TmaAOV4SJNQ">Rosalyne died in a foreign land... But you heartless businessmen and dignitaries, always with a convenient excuse to remain in the comfort of your homeland... You couldn't hope to understand. So why don't you keep your mouths shut! We don't want to make the children cry...</blockquote>
```

## `<q>`
- Defines a short quotation
- Browsers normally insert quotation marks around the quotation.
- Example: 
```html
<q>Rosalyne died in a foreign land... But you heartless businessmen and dignitaries, always with a convenient excuse to remain in the comfort of your homeland... You couldn't hope to understand. So why don't you keep your mouths shut! We don't want to make the children cry...</q>
```

## `<abbr>`
- Defines an abbreviation or an acronym
- Can give useful information to
  - Browsers
  - Translation systems
  - Search engines
- Using the `title` attribute so the description of the abbreviation or acronym when mousing over the element is good practice
- Example:
```html
<abbr title="House of the Hearth">HotH</abbr>
```

## `<address>`
- Defines contact information for the author/owner of an article
- Can be
  - Email address
  - URL
  - Physical address
  - Phone number
  - Social media handle
  - And more
- Text in the `<address>` element usually renders in italic
- Browsers will always add a line break before and after the `<address>` element

## `<cite>`
- Defines the title of a creative work
- A person's name is not the title of the work
- Text in the `<cite>` element usually renders in *italic*
- Example:
```html
<cite>Trofin Snezhevich</cite>, Tattered Paper
```

## `<bdo>`
- BDO stands for Bi-Directional Override
- The `<bdo>` is used to override the current text direction
- Example:
```html
<bdo dir="rtl">This text will be written from right to left</bdo>
```

# [Comments](https://www.w3schools.com/html/html_comments.asp)
- Not displayed in the browser
- Can help document the source code
- Example:
```html
<!-- This is a comment -->
```
- There is an exclamation mark in the start tag, but not the end tag
- Can help to hide content
- Example:
```html
<p>This is a paragraph.</p>

<!-- <p>This is a paragraph that has been commented out</p>

<p>This is another paragraph that has been commented out </p> -->

<p>This is also a paragraph</p>
```
- Parts in the middle of the HTML code can be hidden as well
- Example:
```html
<p>This <!-- comment --> is in a paragraph.</p>
```

# [Colours](https://www.w3schools.com/html/html_colors.asp)

## Colour Names
- Colour can be specified using colour names
- There are 140 standard colour names
- Complete list can be seen [here](https://www.w3schools.com/colors/colors_names.asp)

## Background Colour
- Can be set using the CSS property `background-color`
- Example:
```html
<p style="background-color: #42BC9C">This is a paragraph</p>
```

## Text Colour
- Can be set using the CSS property `color`
- Example:
```html
<p style="color: #42BC9C;">This is a paragraph</p>
```

## Border Colour
- Can be set using the CSS property `border`
- Example:
```html
<p style="border: 2px solid #42BC9C;">This is a paragraph</p>
```

## Colour Values
- Colours can be specified in the following ways
  - RGB
  - HEX
  - HSL
  - RGBA
  - HSLA
- The A in RGBA and HSLA stands for Alpha, which controls the opacity
- For example, the colour #42BC9C is
  - rgb(66, 188, 156)
  - #42BC9C
  - hsl(164, 48%, 50%)
  - rgba(66, 188, 156, 1)
  - hsla(164.26, 48.03%, 49.8%, 1)

### [RGB](https://www.w3schools.com/html/html_colors_rgb.asp)
- RGB represents the **R**ed, **G**reen and **B**lue light sources
- RGBA is an extension of RGB
- In HTML, colour can be specified as a RGB value in this form
```
rgb(red, green, blue)
```
- Each parameter (red, green and blue) defines the intensity of the colour of the value between 0 and 255
- To display black, all parameters are set to 0
- To display white, all parameters are set to 255
- Shades of grey are often defined using equal values for all 3 parameters

### RGBA Colour Values
- In HTML, colour can be specified as a RGBA value in this form
```
rgba(red, green, blue, alpha)
```
- The alpha parameter is a number between 0.0 (Fully transparent) and 1.0 (Fully opaque)

### [HEX](https://www.w3schools.com/html/html_colors_hex.asp)
- In HTML, colour can be specified as a **HEX**adecimal colour in this form
```
#RRGGBB
```
- RR is the hexadecimal integer of the red component of the colour
- GG is the hexadecimal integer of the green component of the colour
- BB is the hexadecimal integer of the blue component of the colour
- Hexadecimal integers can take in values from 00 to FF (Same as decimal 0 to 255)
- To display black, all parameters are set to 00
- To display white, all parameters are set to FF
- Shades of grey are often defined using equal values for all 3 parameters

### [HSL](https://www.w3schools.com/html/html_colors_hsl.asp)
- HSL represents the **H**ue, **S**aturation and **L**ightness
- HSLA is an extension of HSL
- In HTML, colour can be specified as a HSL value in this form
```
hsl(hue, saturation, lightness)
```
- Hue is a degree on the colour wheel from 0 to 360
  - 0 is red
  - 120 is green
  - 240 is blue
- Saturation is a percentage value
  - 0% means a shade of grey
  - 100% is the full colour
- Saturation can also be used to describe the intensity of a colour
  - 100% is the pure colour and there are no shades of grey
  - 50% is 50% gray but you can still see the colour
  - 0% is completely gray and you can no longer see the colour
- Lightness is also a percentage value
  - 0% is black
  - 100% is white
- Lightness can also be used to describe how much light you want to give the colour
  - 0% means no light (Black)
  - 50% means light (Neither dark nor light)
  - 100% meens full lightness (White)
- Shades of gray are often defined by setting the Hue and Saturation to 0, and adjusting the lightness from 0% to 100% to get darker/lighter shades

### HSLA
- In HTML, colour can be specified as a HSLA value in this form
```
hsla(hue, saturation, lightness, alpha)
```

# [CSS](https://www.w3schools.com/html/html_css.asp)
- Stands for **C**ascading **S**tyle **S**heets
- Used to format the layout of a web page
- It is cascading as a style applied to a parent element will apply to all children elements within the parent

## Using CSS
- Can be added in 3 ways
  - Inline
    - Using the `style` attribute inside HTML elements
  - Internal
    - Using a `<style>` element in the `<head>` section
  - External
    - Using a `<link>` element to link an external CSS file
    - Most common way

### Inline CSS
- Used to apply a unique style to a single HTML element

### Internal CSS
- Used to define a style for a single HTML page

### External CSS
- Used to define a style for many HTML pages
- The external file must not contain any HTML code
- It must also end with .css
- Can be referenced with a full URL or with a path relative to the current web page
  - Full URL
    - `https://Venti1707.GitHub.io/external-css.css`
  - Located in an external folder
    - `/css/external-css.css`
  - Located in the same folder
    - `external-css.css`

### Commonly Used CSS Properties
- `color` defines the text colour to be used
- `font-family` defines the font to be used
- `font-size` defines the text size to be used
- `border` defines a border around the HTML element
- `padding` defines a padding (space) between the text and the border
- `margin` defines a margin (space) outside the border

# [Links](https://www.w3schools.com/html/html_links.asp)
- `<a>` tag defines a hyperlink
- Has the following syntax
```html
<a href="url">Text</a>
```
- By default, links will appear as follows in all browsers
  - Unvisited links are underlined and blue
  - Visited links are underlined and purple
  - Active links are underlined and red
- You can style links with CSS

## The `target` Attribute
- Specifies where to open the linked document
- Can have one of the following values
  - `_self`
    - Is the default value
    - Opens in the same window/tab it was clicked
  - `_blank`
    - Opens in a new window/tab
  - `_parent`
    - Opens in the parent frame
  - `_top`
    - Opens in the full body of the window

## Absolute URLs vs Relative URLs
- Absolute URLs are full web addresses
- Relative URLs are local links (They link to a page within the same website, and usually do not include the https://www part)

## Using Images As Links
- Put the `<img>` tag inside the `<a>` tag

## Using Links To Send Emails
- Use `mailto:` inside the `href` attribute to open the user's email program for them to send an email

## The `title` Attribute
-  Specifies extra information about an element
-  Most often shown as a tooltip text when the mouse hovers over said element

## [Link Colours](https://www.w3schools.com/html/html_links_colors.asp)
- Can be styled using CSS

## [Link Bookmarks](https://www.w3schools.com/html/html_links_bookmarks.asp)
- Used so readers can jump to specific parts of a web page
- Can be useful if the web page is very long
- To create a bookmark, perform the following steps:
  - Use the `id` attribute to create a bookmark
    ```html
    <p id="example">Example</p>
    ```
  - Then add a link to the bookmark from within the same page
    ```html
    <a href="#example">Jump to Example</a>
    ```
- You can also add a link to a bookmark on another page
  ```html
  <a href="another-web page.html#example">Jump to Example on another page</a>
  ```

# [Images](https://www.w3schools.com/html/html_images.asp)
- The `<img>` tag is used to embed an image in a web page
- It creates a holding space for the referenced image
- It has 2 required attributes
  - `src`
    - Specifies the path (URL) to the image
  - `alt`
    - Specifies an alternate text to the image
    - Only shown under one of the following conditions
      - There is slow connection
      - An error in the `src` attribute
      - The user uses a screen reader
- Images are not technically inserted in a web page, but instead linked to web pages
- You can also use the `style` attribute to specify the width and height of an image
- You can also use the `width` and `height` attributes
- It is preferred to use the `style` attribute as it prevents CSS files from changing the size of images
- HTML allows for animated GIFs
- Common Image Formats

| Abbreviation | File Format                           | File Extension                   |
| :----------: | :-----------------------------------: | :------------------------------: |
| APNG         | Animated Portable Network Graphics    | .apng                            |
| GIF          | Graphics Interchange Format           | .gif                             |
| ICO          | Microsoft Icon                        | .ico, .cur                       |
| JPEG         | Joint Photographic Expert Group image | .jpg, .jpeg, .jfif, .pjpeg, .pjp |
| PNG          | Portable Network Graphics             | .png                             |
| SVG          | Scalable Vector Graphics              | .svg                             |

## [Image Map](https://www.w3schools.com/html/html_images_imagemap.asp)
- The `<map>` tag defines an image map
- An image map is an image with clickable areas
- The areas are defined with one or more `<area>` tags
- To create one, you need an image and some HTML code that describes the clickable areas

### How To Create An Image Map
- Insert an image using the `<img>` tag
- Add the `usemap` attribute
  - The value starts with a `#` followed by the name of the image map
  - It is used to create a relationship between the image and image map
  - Example:
  ```html
  <img src="Venti.jpg" alt="Venti" usemap="#Venti">
  ```
- Then, add a `<map>` element, where it is then linked to the image with the `name` attribute (they must be the same)
  ```html
  <map name="Venti">
  ```
- Then, add clickable areas by using the `<area>` element
- To define the shape of the clickable area add the `shape` attribute with any of the following values
  - `rect`
    - A rectangular region
    - The coordinates comes in pairs
      - One for the x-axis
      - Another for the y-axis
    - This is then specified as a value in the `coords` attribute like this: `x1, y1, x2, y2`
  - `circle`
    - A circular region
    - Locate the coordinates of the center of the circle, then specify the radius of the circle
    - This is then specified as a value in the `coords` attribute like this: `x, y, radius`
  - `poly`
    - A polygonal region
    - Contains several coordinate points
    - Creates a shape formed with straight lines
    - Can be used to create any shape
    - This is then specified as the value in the `coords` attribute like this: `x1, y1, x2, y2, x3, y3 ..., xn, yn`
  - `default`
    - The entire region

### Image Map & JavaScript
- A clickable area can also trigger a JavaScript function

## Background Images
- Use the `style` attribute and the CSS `background-image` property and add the URL of the image file in `url`
- To avoid the background image from repeating itself
  - Set the `background-repeat` property to `no-repeat`
- To cover the entire element
  - Set the `background-size` property to `cover`
  - Set the `background-attachment` property to `fixed`
- To stretch the entire element
  - Set the `background-size` property to `100% 100%`

## The `<picture>` Element
- Allows you to display different pictures for different devices or screen sizes
- Also gives web developers more flexibility in specifying image resources
- Contains one or more `<source>` elements
- Each refers to different images through the `srcset` attribute
- This way the browser can choose the image that best fits the current and/or device
- Each `<source>` element has a `media` attribute that defines when the image is the most suitable
- Always specify the `<img>` element as the last child element of the `<picture>` element
- The `<img>` element is used by browsers that do not support the `<picture>` element
- Two main reasons for using the `<picture>` element
  - Bandwidth
    - Having a small screen or device means it is not necessary to load a large image file
    - The browser will use the first `<source>` element with matching attribute values and ignore any of the following elements
  - Format Support
    - Some browsers may not support all image formats
    - By using the `<picture>` element, you can add images of all formats, the browser will use the first format it recognizes, and ignore any of the following elements

# Favicon
- Favicon is a small image
- It is displayed next to the page title in the browser tab
- Can be added to the page by using the `<link>` element after the `<title>` element
- Example:

## Favicon File Format Support

| Browser | ICO   | PNG   | GIF   | JPEG  | SVG   |
| :-----: | :---: | :---: | :---: | :---: | :---: |
| Edge    | Yes   | Yes   | Yes   | Yes   | Yes   |
| Chrome  | Yes   | Yes   | Yes   | Yes   | Yes   |
| Firefox | Yes   | Yes   | Yes   | Yes   | Yes   |
| Opera   | Yes   | Yes   | Yes   | Yes   | Yes   |
| Safari  | Yes   | Yes   | Yes   | Yes   | Yes   |

# [Tables](https://www.w3schools.com/html/html_tables.asp)
- Allows web developers to arrange data into rows and columns
- To make a HTML table, follow these steps
  - Start with a `<table>` element
  - Add a header with the `<th>` element
    - `th` stands for **t**able **h**eader
  - Add rows with the `<tr>` element
    - `tr` stands for **t**able **r**ow
    - You can have as many rows as you like in a table
    - Make sure that the number of cells are the same in each row
  - Add content with the `<td>` element
    - `td` standsfor **t**able **d**ata
- You can add more to a table with these elements
  - A caption with the `<caption>` element
    - It should be inserted immediately after the `<table>` element
  - A group of 1 or more columns (as a container of sorts) with the `<colgroup>` element
  - Column properties for each column within a `<colgroup>` element with the `<col>` element
    - The `span` attribute specifies how many columns get the style
    - The `style` attribute specifies the style to give the column
      - You can only use these CSS properties
        - [width](https://www.w3schools.com/cssref/pr_dim_width.php)
        - [visibility](https://www.w3schools.com/cssref/pr_class_visibility.php)
        - [background](https://www.w3schools.com/cssref/css3_pr_background.php)
        - [border](https://www.w3schools.com/cssref/pr_border.php)
  - Group the header content in a table with a `<thead>`
  - Group the body content in a table with a `<tbody>`
  - Group the footer content in a table with a `<tfoot>`

## [Table Borders](https://www.w3schools.com/html/html_table_borders.asp)
- To add a border, use the CSS `border` property on `table`, `th` and `td` elements
- Simple border example:
```css
table, th, td {
  border: 1px solid black;
}
```

- Collapsed border example:
```css
table, th, td{
  border-collapse: collapse;
}
```

- Invisible border example:
```css
table, th, td {
  border: 1px solid /* Colour of the background */;
  border-collapse: collapse;
}

th, td {
  background-color: /* Any colour */;
}
```

- Round border example:
```css
table, th, td { /* You can skip the border around the table by leaving out the table */
  border: 1px solid black;
  border-radius: 10px;
}
```

- Other border styles example:
```css
th, td {
  border-style: /* One of the following: dotted, dashed, solid, double, groove, ridge, inset, outset, none, hidden */;
}
```

## [Table Sizes](https://www.w3schools.com/html/html_table_sizes.asp)
- Use the `style` attribute with the `width` and `height` properties to specify the size of
  - A table
  - A row
  - A column
- Using a percentage as the size unit for a width means how wide the element will be compared to the parent element
- To set the size of a specific column, add the `style` attribute on a `<th>` or `<td>` element

## [Table Headers](https://www.w3schools.com/html/html_table_headers.asp)
- Define the first cell in each row as a `<th>` element
- To align the table headers, use the CSS `text-align` element on the `<th>` element
- To have a header that spans over 2 or more columns, use the `colspan` attribute on the `<th>` element

## [Padding & Spacing](https://www.w3schools.com/html/html_table_padding_spacing.asp)
- Cell padding is the space between the edges and the cell content
- The default padding is set to 0
- To add padding, use the CSS `padding` property
- To add padding to a certain direction relative to the content, use one of the following properties
  - Above the content: `padding-top`
  - Below the content: `padding-bottom`
  - To the left of the content: `padding-left`
  - To the right of the content: `padding-right`
- Cell spacing is the space between each cell
- The default space is set to 2 pixels

## [Colspan & Rowspan](https://www.w3schools.com/html/html_table_colspan_rowspan.asp)
- HTML tables can have cells that span over multiple rows and/or columns

## [Table Styling](https://www.w3schools.com/html/html_table_styling.asp)
- To add horizontal stripes on every even/odd table row, use the `:nth-child()` selector like this
```css
tr:nth-child(even) { /* This is for every row number that is even */
  background-color: /* Any colour */
}

tr:nth-child(odd) { /* This is for every row number that is odd */
  background-color: /* Any colour */
}
```
- To add vertical stripes on every even/odd table column, use the `:nth-child()` selector like this
```css
td:nth-child(even), th:nth-child(even) { /* This is for every column number that is even */
  background-color: /* Any colour */;
}

td:nth-child(odd), th:nth-child(odd) { /* This is for every column number that is odd */
  background-color: /* Any colour */;
}
```
- To combine both to get stripes on every even row, use the `:nth-child()` selector like this
```css
tr:nth-child(even) {
  background-color: /* Any colour */;
}

th:nth-child(even),td:nth-child(even) {
  background-color: /* Any colour */;
}
```
- To get horizontal stripes, add the `:hover` selector to all `tr` elements like this
```css
tr:hover {
  background-color: /* Any colour */;
}
```

# [Lists](https://www.w3schools.com/html/html_lists.asp)
- Lists allow web developers to group a set of related items in lists
- Unordered lists start with the `<ul>` tag
- Ordered lists start with the `<ol>` tag
- Each list item starts with the `<li>` tag
- HTML also supports description lists
- Description lists is a list of terms, with a description of each term.
- The `<dl>` tag defines the description list
- The `<dt>` tag defines the tag name
- The `<dd>` tag describes each term

## [Unordered Lists](https://www.w3schools.com/html/html_lists_unordered.asp)
- The CSS `list-style-property` is used to define the style of the list item marker
- It can have one of the following values
  - `disc` (This is the default value)
  - `circle`
  - `square`
  - `none`
  - More can be seen [here](https://www.w3schools.com/cssref/pr_list-style-type.php)

## [Ordered Lists](https://www.w3schools.com/html/html_lists_ordered.asp)
- The `type` attribute of the `<ol>` tag is used to define the type of the list item marker
- It can have one of the following values
  - `type="1"` (The is the default value)
    - The list items will be numbered with numbers (default)
  - `type="A"`
    - The list items will be numbered with uppercase letters
  - `type="a"`
    - The list items will be numbered with lowercase letters
  - `type="I"`
    - The list items will be numbered with uppercase roman numbers
  - `type="i"`
    - The list items will be numbered with lowercase roman numbers