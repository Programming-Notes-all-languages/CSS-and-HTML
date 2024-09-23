<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#comments'>Comments</a>
  </li> 
  <li>
    <a href='#css-selectors'>CSS Selectors</a>
  </li> 
  <li>
    <a href='#external-internal-and-inline-css'>External, Internal, and Inline CSS</a>
  </li>
</ol>
</details> 

## Comments
<ul>
  <li>
    <a>A single line comment is the following in CSS: /* This is a single-line comment */</a>
  </li>
  <li>
    <a>A multi-line comment is the following in CSS: /* This is<br>a multi-line<br>comment */</a>
  </li>
</ul>      

## CSS Selectors
<ul>
  <li>
    <a>Here is the syntax for a CSS selector: className {<br>
    &nbsp;&nbsp;&nbsp;&nbsp;propertyName: value;<br> 
    }</a>
  </li>
  <li>
    <a>The name of the class can be named with the same tag as a section of code within the html file. Class attributes, for instance, within the body class in the css file, will reflect in the encapsulated code within the <a><</a>body<a>></a> tag and the <a><</a>/body<a>></a> tag</a>
  </li>
  <li>
    <a>To create a class where all elements with the class attribute can be modified by a class, the period (.) can be applied before the name of the class</a>
    <ul>
      <li>
        <a>For instance, if a class has the following declaration:

```css
.gray {
color: gray;
}
```

then any section of the code within the html file can obtain the attributes defined within the class if the class attribute is included after within the html tag. This is accomplished by proceeding the name of the tag within the arrow with the following: <a><</a>tagName class="className"<a>></a>. This is only needed in the opening tag--not in the closing tag</a>
      </li>
    </ul>
  </li>  
  <li>
    <a>A class with the name * is a universal class that applies to all elements within the html file. This class is like a parent/base class that applies to all</a> 
    <ul>
      <li>
        <a>Here is an example of a universal class:

```css 
* {
    color: #820025;
    background: rgb(131, 127, 100);
}
```

all elements within the html file will have the text color #820025 and a background color of that rgb value</a>
</li></ul></li>  <li>
    <a>The grouping selector can be used when multiple HTML elements are desired to share the same class definitions</a>
    <ul>
      <li>
        <a>Here is an example of a grouping selector:

```css
h1, h2, p {
    text-align: center;
    color: red;
}
```
Now, h1, h2, and p all have their text aligned to the center and all of the text within the tags is red</a>
</li>  </ul>
</li>
  <li>
    <a>There is even functionality to specify with HTML elements will be affected by the implementation of a class</a>
    <ul>
      <li>
        <a>The syntax for this is the following:

```css
p.center {
    text-align: center;
    color: red;
}
```
only p elements within the HTML file will be affected by the center class</a></li></ul></li>
</ul>  

## External, Internal, and Inline CSS
<ul>
  <li>
    <a>There are three ways to insert a style sheet within a .html file: external, internal, and inline</a>
  </li>
</ul>  

### External CSS
<ul>
  <li>
    <a>When using an external style sheet, the look of a website can be modified within one .css file</a>
  </li>
  <li>
    <a>Each .html file working to create the website must be linked inside of each head section within each .html file</a>
    <ul>
      <li>
        <a>Here is the syntax for how to link a .css style sheet within the head of a .html file: <a><</a>link rel="stylesheet" href="filePath.css"<a>></a></a>  

```html
<!DOCTYPE html>
    <html lang="en">
        <head>
            <meta charset="UTF-8"/>
            <link rel="stylesheet" href="style.css">
            <title>My First Webpage</title>
        </head>
        
        <!-- Header -->
        <header>
            <h1>Welcome to Our Webpage!</h1>
            <p>This is a new webpage created by Garrett Ellis.</p>
        </header>

        <!-- Images -->
        <a href="Images/Horizon.jpg">
            <img src="images/Horizon.jpg" alt="Carnival Horizon">
        </a>
    </html>
```   

```css
header {
    color: #820025;
    background: rgb(131, 127, 100);
}
```
</li></ul></li></ul>

### Internal CSS
<ul>
  <li>
    <a>Internal style sheets can be used within the .html file to modify the contents encapsulated within the HTML elements</a>
  </li>
  <li>
    <a>Internal styles are denoted with the <a><</a>style<a>></a> element that is encapsulated within the head section of the .html file</a>

```html
<!DOCTYPE html>
    <html lang="en">
        <head>
            <meta charset="UTF-8"/>
            <title>My First Webpage</title>
            <style>
                header {
                    color: #820025;
                    background: rgb(131, 127, 100);
                }
            </style>
        </head>
        
        <!-- Header -->
        <header>
            <h1>Welcome to Our Webpage!</h1>
            <p>This is a new webpage created by Garrett Ellis.</p>
        </header>

        <!-- Images -->
        <a href="Images/Horizon.jpg">
            <img src="images/Horizon.jpg" alt="Carnival Horizon">
        </a>
    </html>
```
</li></ul></li></ul>

### Inline CSS
<ul>
  <li>
    <a>Inline CSS can often be useful for modifying a single element within the .html file</a>
    <ul>
      <li>
        <a>Here is an example of using inline CSS to modify a single HTML element while using the style attribute</a>

```html
<!DOCTYPE html>
    <html lang="en">
        <head>
            <meta charset="UTF-8"/>
            <title>My First Webpage</title>
        </head>
        
        <!-- Header -->
        <header style="color: #820025;background: rgb(131, 127, 100);">
            <h1>Welcome to Our Webpage!</h1>
            <p>This is a new webpage created by Garrett Ellis.</p>
        </header>

        <!-- Images -->
        <a href="Images/Horizon.jpg">
            <img src="images/Horizon.jpg" alt="Carnival Horizon">
        </a>
    </html>
```

### Precedence of External Style Sheets, Internal Style Sheets, and Inline Style Sheets
<table>
  <thead>
    <tr>
      <th>Precedence</th>
      <th>Style Sheet Type</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>Inline (inside HTML element)</td>
    </tr>
    <tr>
      <td>2</td>
      <td>External and Internal (in head section)</td>
    </tr>
    <tr>
      <td>3</td>
      <td>Browser Default</td>
    </tr>
  </tbody>
</table>     