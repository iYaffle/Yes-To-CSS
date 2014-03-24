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
This is where the factor of re-usability comes to play. You can apply same set of CSS styles across multiple HTML documents by creating a single .css file. 

Using an external CSS resource can be done either by using &lt;link&gt; tag or using @import keyword in your &lt;style&gt; tag.

Let us see an example for each of these methods. Before going to the example, let's assume we have a file named style.css , which we want to include in our web page. The file has the below content and it's just a plain text CSS code.

```css
p {
  color: red;
  backgroud-color: white;
}
```

Now, we have another file named example.html where we want to use our style.css file. To summarize, We have 2 separate files, one for the content(example.html) layer and one for presentation(style.css) layer.

### Example using &lt;link&gt;: ###

In the below example, the style.css file is linked to the example.html file as a stylesheet. 

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

### Example using @import: ###

Let's do the same thing now but with @import keyword. You can notice that we have used &lt;style&gt; tag instead of &lt;link&gt; tag to import. The file content of style.css does not change. Only the way you include this file to your html file changes.

**example.html**
```html 
<html>

    <head>
        <title>Yes to CSS - Demo</title>
        <style>
           @import url('style.css');
        </style>
    </head>

    <body>
        <p>This text will be in red color</p>
    </body>

</html>
```

The literal meaning of this method is that the style.css file's content is imported to your example.html file.

> **Points to Ponder** 
> Always use &lt;link&gt; tag where ever possible instead of @import keyword when you want to include any external CSS file to your web page. Using @import may create a bottleneck in your web page load time as it does not allow parallel download of files.

Comparison of 3 methods
-----------------------
There are some advantages for using external CSS files because of the following reasons.

 - Page load performance will be better if browsers can cache them.
 - It's very easy for development, maintenance and re-usability. 
 - HTML and styling are separated fully according to general web standards.

In some cases, using inline CSS styles is much appropriate. For example, if you want just to style a single element, there is no point of creating a .css external file. So consider other methods of using CSS based on your requirement and styling complexity. 

Your Comments
-------------
Oh! wait. We are not asking for your comment on this tutorial now. Not yet, buddy. This section tells you how to add some comments to the CSS document. Using comments extensively in any programming is always good for better readability and understanding of the code.

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

You can have the comments spanning multiple lines. In the below example, 2 lines are commented using a single comments block.

```css
p {
  /*color: red;
  backgroud-color: white;*/
}
```

But you **can't** have them nested as below. The below sample CSS is incorrect as it has nested comment blocks.

```css
p {
  /*color: red; /*red color*/
  backgroud-color: white;*/
}
```
