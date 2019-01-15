# html-standards
Coding standards and guide for developing apps using HTML


# HTML5  Style Guide and Coding Conventions

We will follow most the standards suggested by the [w3Schools](https://www.w3schools.com) that can be found [here](https://www.w3schools.com/html/html5_syntax.asp).

They have very simple and easy to understand guides and standard to follow.

  

# HTML Coding Conventions

Web developers are often uncertain about the coding style and syntax to use in HTML.

Between 2000 and 2010, many web developers converted from HTML to XHTML.

With XHTML, developers were forced to write valid and "well-formed" code.

HTML5 is a bit more sloppy when it comes to code validation.

  

## Be Smart and Future Proof

A consistent use of style makes it easier for others to understand your HTML.

In the future, programs like XML readers may want to read your HTML.

Using a well-formed-"close to XHTML" syntax can be smart.

  

Always keep your code tidy, clean and well-formed.

  

## Use Correct Document Type

Always declare the document type as the first line in your document:

  

    <!doctype html>

  

# Indention and spaces

Following the PHP example.

As [PSR-2](https://www.php-fig.org/psr/psr-2/) dictates that indention should be 4 (four blank spaces).

Do not add blank lines without a reason.

For readability, add blank lines to separate large or logical code blocks.

Do not use unnecessary blank lines and indentation. It is not necessary to indent every element:

And every child node should be indented once from parent.

    <!doctype html>
    <html>
    	<body>
    		<h1>My Title</h1>
    		<p>My Paragraph</p>
    	</body>
    </html>

  

# Use Lower Case Element Names

HTML5 allows mixing uppercase and lowercase letters in element names.

We recommend using lowercase element names because:

-   Mixing uppercase and lowercase names is bad
-   Developers normally use lowercase names (as in XHTML)
-   Lowercase look cleaner
-   Lowercase are easier to write

    <section> 
      <p>This is a paragraph.</p>
    </section>

  

# Close All HTML Elements

In HTML5, you don't have to close all elements (for example the  `<p>`  element).

We recommend closing all HTML elements.

  

# Use Lower Case Attribute Names

HTML5 allows mixing uppercase and lowercase letters in attribute names.

We recommend using lowercase attribute names because:

-   Mixing uppercase and lowercase names is bad
-   Developers normally use lowercase names (as in XHTML)
-   Lowercase look cleaner
-   Lowercase are easier to write

    <div class="form-group" id="form-container" data-lower-case-attrib="7">

  

# Quote Attribute Values

HTML5 allows attribute values without quotes.

We recommend quoting attribute values because:

-   Mixing uppercase and lowercase values is bad
-   Quoted values are easier to read
-   You MUST use quotes if the value contains spaces

    <p class="quoted-attribute">

  

# Image Attributes

Always add the  `alt`  attribute to images. This attribute is important when the image for some reason cannot be displayed. Also, always define image width and height. It reduces flickering because the browser can reserve space for the image before loading.

    <img src="html5.gif" alt="HTML5" style="width:128px;height:128px;">

  

# Avoid Long Code Lines

When using an HTML editor, it is inconvenient to scroll right and left to read the HTML code.

Try to avoid code lines longer than 80 characters.

  

# Setting The Viewport

HTML5 introduced a method to let web designers take control over the viewport, through the  `<meta>`  tag.

The viewport is the user's visible area of a web page. It varies with the device, and will be smaller on a mobile phone than on a computer screen.

You should include the following  `<meta>`  viewport element in all your web pages:

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

The initial-scale=1.0 part sets the initial zoom level when the page is first loaded by the browser.

Here is an example of a web page  _without_  the viewport meta tag, and the same web page  _with_  the viewport meta tag:

If you are browsing this page with a phone or a tablet, you can click on the two links below to see the difference

  

# HTML Comments

Short comments should be written on one line, like this:

    <!-- This is a comment -->

Comments that spans more than one line, should be written like this:

    <!-- 
      This is a long comment example. This is a long comment example.
      This is a long comment example. This is a long comment example.
    -->

  

# Style Sheets

Use simple syntax for linking to style sheets (the type attribute is not necessary):

    <link rel="stylesheet" href="styles.css">

Short rules can be written compressed, like this:

    p.intro {font-family: Verdana; font-size: 16em;}

Long rules should be written over multiple lines:

    body {
	    background-color: lightgrey;
	    font-family: "Arial Black", Helvetica, sans-serif;
	    font-size: 16em;
	    color: black;
    }

-   Place the opening bracket on the same line as the selector
-   Use one space before the opening bracket
-   Use two spaces of indentation
-   Use semicolon after each property-value pair, including the last
-   Only use quotes around values if the value contains spaces
-   Place the closing bracket on a new line, without leading spaces
-   Avoid lines over 80 characters

  

# Loading JavaScript in HTML

Use simple syntax for loading external scripts (the type attribute is not necessary):

    <script src="myscript.js">

  

# Accessing HTML Elements with JavaScript

A consequence of using "untidy" HTML styles can result in JavaScript errors.

These two JavaScript statements will produce different results:

    var obj = getElementById("Demo")
    
    var obj = getElementById("demo")

  

# Use Lower Case File Names

Some web servers (Apache, Unix) are case sensitive about file names: "london.jpg" cannot be accessed as "London.jpg".

Other web servers (Microsoft, IIS) are not case sensitive: "london.jpg" can be accessed as "London.jpg" or "london.jpg".

If you use a mix of upper and lower case, you have to be extremely consistent.

If you move from a case insensitive to a case sensitive server, even small errors will break your web!

To avoid these problems, always use lower case file names.

  

# File Extensions

HTML files should have a  **.html**  or  **.htm**  extension.

CSS files should have a  **.css**  extension.

JavaScript files should have a  **.js**  extension

  

----------

  

References:

-   [https://www.w3schools.com/html/html5_syntax.asp](https://www.w3schools.com/html/html5_syntax.asp)


