Come With Flying Colors
=======================

This should be the most colorful section of our guide. Yes, we are going to deal with colors and background of HTML documents.

Color Property
--------------
Assume you have a text paragraph and want to change the text color of it. Of course, you can change the color using &lt;font&gt; tag for that. But remember we are dealing with CSS here.

The below code applies red color for the text within all paragraphs identified by  &lt;p&gt; tag.

```css
p { 
  color: white;
}
```

Or, if you want to apply the color only to a particular element based on a ID or by class, below are the examples.
```css
#div1 { 
  color: white;
}
```
```css
.class1 { 
  color: white;
}
```

This CSS property is only applied to texts.

Background-Color Property
-------------------------
As applying a color to the text, we can also apply background colors to text or any other element.

```css
p { 
  background-color: red;
}
```
As mentioned earlier, the background-color property can be applied to any element of a particular Id or Class.

To create pretty and readable texts, we can combine both the *color* and *background-color* property of the text. The below example present the text in white foreground color and red background color. Is that pretty enough?

```css
p { 
  color: white;
  background-color: red;
}
```

Color Models
------------
CSS provides the flexibility of representing colors in 3 different ways. You can chose to specify a color either in one of the standard formats mentioned below.

 1. Standard color name : *green*
 2. HEX : *#00ff00*
 3. RGB (Red, Green, Blue) : *rgb(0,255,0)*
 4. RGBA (Red, Green, Blue, Alpha) : *rgba(0,255,0,0.3)*
 5. HSL (Hue , Saturation, Lightness) : *hsl(120,100%,75%)*
 6. HSLA (Hue , Saturation, Lightness, Alpha) : *hsla(120,100%,75%,0.3)*

> **NOTE:**
>
> - The output of RGB mode is dependent on the hardware, as you can observe the color differences in different quality of monitors.
> - The RGB values have a range from 0-255.
> - HSL color mode depends on the light exposure and considered better for use over RGB scheme.
> - Hexadecimal color code always start with an #. Refer above exammple.

Below are the examples showing the use of different color schemes using along with H2 tag.

**Color Name:**

```css
h2 {
   color: black;
}
``` 

**HEX Code:**

```css
h2 {
   color: #ff0000;
}
``` 

**RGB Mode:**
```css
h2 {
   color: rgb(100,255,100);
}
``` 

**RGBA Mode:**
```css
h2 {
   color: rgba(100,255,100,0.5);
}
``` 

**HSL Mode:**
```css
h2 {
   color: hsl(120,90%,90%);
}
``` 

**HSLA Mode:**
```css
h2 {
   color: hsla(100,90%,75%,0.7);
}
``` 

Transparent Colors!
-------------------

If you want to try a transparent color, you can either use the color name as "*transparent*" or rgba(0,0,0,0) which denotes transparent black color.

Below are the two variants of using transparent colors.
```css
h2 {
   color: transparent;
}
``` 

```css
h2 {
   color: rgba(0,0,0,0);
}
```
There are few other descriptive values in CSS and are covered in the below sections.

> **NOTE 1:**
>
> The 6 digit HEX code can also be represented in 3 character short form. For example, the color #09C is equivalent to #0099CC in CSS.

> **NOTE 2:**
>
> The 3 digit HEX code is valid only in CSS and will not be applied in HTML inline styles. Using 3 digit codes limit the number of colors to 4096 which is highly enough for common colors.

Using CurrentValue
------------------

> **TIPS:** Several online tools are available to convert color codes from
> one format to another. These tools comes really handy when looking for
> some wierd colors like *FireBrick*, *OldLace* and *NavajoWhite*. Hope
> you will be using them too :)

Using Inherit
-------------

> **TIPS:** It's always safe to use shades of green, yellow, and blue colors as they are called as "really safe" colors; Some colors does
> not look same on all browsers.

Here we go. We are end of our chapter on CSS Colors and sure you have already tried to see what does the color *NavajoWhite* looks like. Cheers!!!
