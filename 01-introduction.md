Introduction to CSS
===================

Assumption
----------
This guide assumes that the reader is aware of some basic HTML. Although recommended, knowing basics of web programming language like PHP, Java Script will be an added advantage.

This guide has been organized in a simple manner so that its easy to follow even for a rookie designer who doesn't have any prior experience on HTML and CSS.

Secrets About HTML
------------------
To use CSS, you obviously need some amount of HTML to play around. If you are new to web development, this section will help you understand about HTML in high level.

What is CSS?
------------
Let us start with understanding what is CSS and what it can do for us.

CSS is the acronym for *Cascading Style Sheet*. Let's break these 3 words and explain each of them in reverse for better understanding.

> **Sheet** - a document or a file or a chunk of text following a syntax

> **Style** - the way of formatting or representing the HTML content

>**Cascading** - applying the above mentioned styles in a defined order based on priority

To start, CSS is a file or some texts which is used to format the content in HTML. Let's see couple of examples which will help you to understand what was just explained. If you do not follow the syntax or the meaning, don't feel frustrated. By the end of the section, you will be able to.

The below mentioned file with a ".css" extension is a CSS file.

> C:\Files\iyaffle.css

The below code chunk found in an HTML document is also called CSS.

```html
<style>
    P {
      color: red;
    }
</style>
```

The browsers like FireFox, Chrome & Opera (I didn't forget IE) reads these and based on those, renders the HTML content with awesome styles and shows you. The same happens for any website that you read, say www.google.com or www.facebook.com. All these websites has some CSS files or styles included in their HTML content.

> **TIPS :** To view the HTML code (and CSS), right click on any web page and click "View Page Source" menu. The menu text might change from
> browser to browser, but the concept is same.

Yet, we have not covered what *Cascading* refers to. Well, here we go.

In a HTML document, there is a possibility that you might be trying to include many CSS files or styles from different developers/designers, which often happens in a larger project.

The cascade is about what take precedence when there is a conflict. The rules of the cascade include:

- Later properties override earlier properties
- More specific selectors override less specific selectors
- Specified properties override inherited properties


Why CSS?
--------
This section will answer to your question of *Why do we need CSS*?

What you will love?
-------------------
Some advantages of using CSS

HTML and CSS
------------
What's the relationship of CSS with HTML?

CSS Speciciations
-----------------

CSS1
CSS2
CSS3
