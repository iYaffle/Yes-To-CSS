Come With Flying Colors
=======================

This should be the most colorful section of our guide. Yes, we are going to deal with colors and background of HTML documents.

Color Property
--------------

Color Modes
-----------
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

If you want to try a transparent color, you can either use the color name as "transparent" or rgba(0,0,0,0) which denotes transparent black color.

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

