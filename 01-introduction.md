Introduction to CSS
===================

Assumption
----------
This guide assumes that the reader is aware of some basic HTML. You don't need to have any knowledge of programming languages like PHP or .NET, but if you do know you can quickly pick up the concepts.

This guide has been organized in a simple manner so that its easy to follow even for a rookie designer who doesn't have any prior experience on CSS.

Secrets About HTML
------------------
To use CSS, you obviously need some amount of HTML to play around. If you are new to web development, this section will help you understand about HTML in high level.

In the words of W3C,

> HTML is the language for describing the structure of Web pages.

In our words, HTML is used to create a structured layout of your content which is easy to maintain(to some extend) and publish online. 

Tim Berners-Lee was the man who changed the world by inventing HTML in 1990. The initial purpose of HTML was to help scientist share their findings and research documents with others. Later it has evolved to what we call now as *Web*. People started to share personal information and other kinds of textual information. As more and more data gets added, it's required to "mark-up" the document for easy understanding.

For example, if you want to highlight a heading in a document, you use a specific syntax( or called as tags). This way, more structure document can be created.

Again make a note that this guide assumes that the reader has some knowledge on HTML.

What is CSS?
------------
Let us start with understanding what is CSS and what it can do for us.

CSS is the acronym for *Cascading Style Sheet*. Let's break these 3 words and explain each of them in reverse for better understanding.

> **Sheet** - a document or a file or a chunk of text following a syntax

> **Style** - the way of formatting or representing the HTML content

>**Cascading** - applying the above mentioned styles in a defined order based on priority

To start, CSS is a way of telling your browser how to show the HTML content to your eyes. CSS, basically can be either as a file or some texts which follows a particular syntax. Let's see couple of examples(as a file, as text chunk) which will help you to understand what was just explained. 

The below mentioned file with a ".css" extension is a CSS file.

> C:\Files\style.css

The below code chunk found in an HTML document is also called CSS.

```html
<style>
    P {
      color: red;
    }
</style>
```
If you do not follow any syntax or the meaning, don't feel frustrated. By the end of the section, you will be able to.

The browsers like FireFox, Chrome & Opera (I didn't forget IE) reads these and based on those, renders the HTML content with awesome styles and shows you. The same happens for any website that you read, say www.google.com or www.facebook.com. All these websites has some CSS files or styles included in their HTML content.

> **TIPS :** To view the HTML code (and CSS), right click on any web page and click "View Page Source" menu. The menu text might change from
> browser to browser, but the concept is same.

Yet, we have not covered what *Cascading* in the acronym refers to. Well, here we go.

In a HTML document, there is a possibility that you might be trying to include many CSS files or styles from different developers/designers, which often happens in a larger project.

The cascade is about what take precedence when there is a conflict. The rules of the cascade include:

- Later properties override earlier properties
- More specific selectors override less specific selectors
- Specified properties override inherited properties

HTML and CSS
------------
Are you wondering the relationship between CSS with HTML? If not you skip this section.

HTML is the language using which you specifiy your web page content and how they are structured. 

CSS is the language using which you describe the presentation of web page content by using colors, fonts and various other design concepts. 

Whether you browse the web page in your Windows Desktop or in your Nokia Lumia or in your iPhone 5, the content is not going to change. But by using CSS, you can make your web pages to adapt the formatting of content based on the devices.

so, HTML is like a raw product and CSS is the packaging method. As you can gift-pack a product with different designs, you can make a web page look different by using different CSS styles.

The main purpose of CSS is to take out the presentation logic from HTML document content. Re-usablity of CSS code across multiple web pages can also be achieved by seperating them.

> **TIP:** If you are .NET or a PHP developer, you should have an idea of MVC frameworks which separates the View and Controllers. It's the same with HTML and CSS.


What you will love in CSS?
--------------------------
This section will answer to your question of *Why do we need CSS*?

 - A clear separation of markup vs styles
 - cleaner HTML markup

> **Do You Know?** 
> CSS was initially called as CHSS(Cascading *HTML* Style Sheets). But later as style sheets can be used for other structured documents like XML, the *HTML* was eventually dropped.

CSS Specifications
------------------
We just saw  that all web browsers use CSS to show the styled content to end users. Web browsers are developed by different vendors. Below are some common web browsers and their vendor.

 - **Chrome** by *Google*
 - **FireFox** by *Mozilla*
 - **Internet Explorer** by *Microsoft*
 - **Opera** by *Opera Software*
 - **Safari** by *Apple*

To provide a standard browsing experience, your web pages should look similar in all browsers. To achieve this all web browsers should follow a common standards for rendering the HTML document. So who is that big guy to define standards for CSS? It's the W3C (World Wide Web Consortium) who does the work for us.

The W3C has created multiple version of CSS specifications and the major versions are called CSS1, CSS2 and CSS3. Each version has new features and some changes over the old version.

Details on each of these specifications itself can be a separate book on its own. so we will be just covering some basic stuffs on them.

### CSS1 ###
The CSS level 1 specification was first published in 1996 and now most browsers support all features of CSS3. Basic support for Fonts, Colors and Text properties were present in this.

### CSS2 ###
Version 2 was published on 1998 and it added advanced properties for element positioning, Fonts and media types.

### CSS3 ###
This is the current recommended version of CSS and all other older versions are not maintained. Initial specification was published in 1999 and new capabilities are getting added to the formal recommendation.

### CSS4 ###
CSS4 is an in-progress version. The future proposal will have many new features and there is no clarity on its changes/enhancements. We do not cover any of its feature in this guide. Let's cross our fingers for it.

> **NOTE:** There are also some sub-version like CSS 2.1 which is also no longer maintained as all other old versions.

As CSS3 is the current recommended specification, whenever we mention CSS, it refers to CSS3 unless until we say otherwise.
