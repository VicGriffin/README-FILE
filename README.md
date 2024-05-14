<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents** 

- [CSS BOX MODEL DOCUMENTATION](#css-box-model-documentation)
  - [CSS sytanx](#css-sytanx)
  - [CSS selectors](#css-selectors)
    - [ways to declare css file](#ways-to-declare-css-file)
    - [Components of the CSS Box Model](#components-of-the-css-box-model)
    - [Box model diagram](#box-model-diagram)
    - [Example](#example)
  - [Width and Height of an Element](#width-and-height-of-an-element)
    - [Example](#example-1)
    - [Conclusion](#conclusion)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# CSS BOX MODEL DOCUMENTATION

## CSS sytanx
-consists of a selector and a declaration block example
```css
body{color:red#;
     border: none;
    padding: none;
    box-sizing: border-box;
}   
```
on the code above you notice there are styles put in place that help edit the body( which is the selector)
and color, border, padding, box-sizing (which can be said to be declaration) give the property and a value for styling
## CSS selectors
-There are various types of selector i.e
- simple selctors
- combinator selectors
- group selectors
- tag selectors
- class selectors
- universal selectors

  
### ways to declare css file
- inline   
inline elements are elements that do not start on a new line and only take up as much width as necessary. 
```html
<p style="color: red; "> play hard give more</p>
```
- internal   
Internal CSS involves embedding CSS rules directly within the head section of an HTML document using the style tag
```html
<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```
- external   
External CSS involves linking to an external CSS file from the HTML document using the link tag. 
```html
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="style.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>  
```

```css
body{color:red#;
     border: none;
    padding: none;
    box-sizing: border-box;
} 
```
### Components of the CSS Box Model
1. Content: this is where the text, images, or other content is displayed. it is Controlled by properties like width and height.
1. padding: This is the space between the content and the border of the box. It creates space inside the box, around the content. for example we can have properties like padding-top, padding-right, padding-bottom, padding-left, or the shorthand padding.
1. Border: this is a line that surrounds the padding and content where border can be styled, sized, and colored. some of the properties includes border-width, border-style, border-color, or the shorthand border.  
1. Margin: The space outside the border, separating the element from other elements. Margins can be used to create space between elements.  

### Box model diagram
![css box model](./assets/box%20mode.jpg)

The box model allows us to add a border around elements, and to define space between elements.   
### Example
Demonstration of the box model:

```css
div {
  width: 300px;
  border: 15px solid green;
  padding: 50px;
  margin: 20px;
}
```
## Width and Height of an Element
you need in order to set the width and height of an element correctly in all browsers.  
### Example
This is a div element will have a total width of 350px and a total height of 80px: 
```css
div {
  width: 320px;
  height: 50px;
  padding: 10px;
  border: 5px solid gray;
  margin: 0;
}
``` 
### Conclusion
Understanding the CSS box model is essential for web development. It allows you to manipulate the spacing, size, and layout of elements accurately. By mastering properties like padding, border, margin, and box-sizing, you can create precise and well-structured web designs.


7/7





