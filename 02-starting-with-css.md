Starting With CSS
=================

Basic CSS Syntax
----------------
Let's now start with the basic usage of CSS in our HTML files. You need to understand that CSS can't exists without HTML. They are made for each other :) Said that, we have to place our CSS styles in the HTML file. Based on where we place those CSS code, we can have 3 different ways of using CSS, which are listed below.

 1. Inline CSS 
 2. Internal CSS 
 3. External CSS

What ever way you choose to use, each have its own up and down side. Let us see about each one of those types.

Inline CSS
-------------
How to use inline CSS

```html
<html>

    <head>
        <title>Yes to CSS - Demo</title>
    </head>

    <body>
        <p style="color:red;">This text will be in red color</p>
    </body>

</html>
```
You can use multiple properties by separating them with comma as shown below.

    <p style="color:red;background-color:white;">Red in White</p>

The re-usability of inline CSS is 0% and can be used when you want to override some global styles applied by other 2 methods.

Internal CSS
-------------
They are also called *Embedded CSS* by some folks. These types of CSS are included in the &lt;head&gt; section of the HTML document within the &lt;style&gt; tag.

```html
<html>

    <head>
        <title>Yes to CSS - Demo</title>

        <style type="text/css">
           p {
              color: red;
           }
        </style>

    </head>

    <body>
        <p>This text will be in red color</p>
    </body>

</html>
```

As you see in the above example, the CSS style code is embedded to the document by using &lt;style&gt; tag which in turn is placed in the &lt;head&gt; tag.

> **Points to Ponder** 
> These kind of CSS styles are applied only to the particular HTML document where it is embedded. If you want to use the same set of styling rules across multiple pages, you need to duplicate them in all HTML documents.

External CSS
-------------
This is where the factor of re-usability comes to play. You can apply same set of CSS styles across multiple HTML documents by creating a single .css file. In the below example, file named style.css is linked to the document as a stylesheet. So we have 2 separate files, one for the content(example.html) layer and one for presentation(style.css) layer.

**example.html**
```html 
<html>

    <head>
        <title>Yes to CSS - Demo</title>
        <link rel="stylesheet" type="text/css" href="style.css">
    </head>

    <body>
        <p>This text will be in red color</p>
    </body>

</html>
```
**style.css**

```css
p {
  color: red;
  backgroud-color: white;
}
```

The css file is nothing but a plain text file which you can edit in a Notepad, with a .css extension.

Comparison of 3 methods
-----------------------
There are some advantages for using external CSS files because of the following reasons.

 - Page load performance will be better if browsers can cache them.
 - It's very easy for development, maintenance and re-usability. 
 - HTML and styling are separated fully according to general web standards.

In some cases, using inline CSS styles is much appropriate. For example, if you want just to style a single element, there is no point of creating a .css external file. So consider other methods of using CSS based on your requirement and styling complexity. 

Your Comments
-------------
Oh! wait. We are not asking for your comment on this tutorial now. Not yet, buddy. This section tells you how to add some comments to the CSS document. Using comments extensively in any programming is always good and advisable.

In CSS to add a comment , start the line with */** and ends with **/*. The below example shows how to do that.

```css
p {
  color: red; /* make text with red font color */
  backgroud-color: white;   /* make text with white backgroud */
}
```
You can also use comments to stop a particular property from being styled.

```css
p {
  color: red;
  /*backgroud-color: white;*/
}
```
