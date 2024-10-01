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
    <a>A single line comment is the following in CSS:</a>

```c
/* This is a single-line comment */
```
  </li>
  <li>
    <a>A multi-line comment is the following in CSS:</a>

```css     
/* This is
a multi-line
comment */
```
  </li>
</ul>      

## CSS Selectors
### The CSS Element Selector
<ul>
  <li>
    <a>When using an element selector, all HTML elements named htmlElements will all be affected by this CSS class. Each property within this class will affect the appearance of text within the named HTML element</a>
  </li>  
  <li>
    <a>Here is the syntax of a CSS element selector:</a> 

```css
htmlElement {
    propertyName: value; 
}
```  
  </li>
</ul>  
  
### The CSS ID Selector
<ul>
  <li>
    <a>The id selector uses the id that is associated with an HTML element to define which HTML elements will be affected by this CSS class</a> 
  </li>
  <li>
    <a>Here is the syntax of a CSS id selector:</a>

```css
#htmlElement {
    propertyName: value;
    propertyName2: value2;
}
```
  </li>
</ul>  

### The CSS Class Selector
<ul>
  <li>
    <a>The class selector is used to modify the HTML elements that have that specific class attribute. Therefore, there can be the same HTML element that is affected by a class selector, but that same HTML element later in the code may not be affected if the specific class attribute is not applied</a>
  </li>
  <li>
    <a>Here is the syntax of a CSS class selector:</a>  

```css
.className {
    propertyName: value;
    propertyName2: value2;
}
```
  </li>
  <li>
    <a>To then apply the class selector to a specific HTML element, the following can be inserted within the elements tag:</a>

```css
<htmlElement class="className">
```
  </li>
    <ul>
      <li>
        <a>The addition of the above within the first opening HTML element is only needed for the first opening tag--not the second closing tag</a>
      </li>
    </ul>    
  </li>
  <li>
    <a>With class selectors, there is functionality to specify which HTML elements should be affected by a class selector. To do that, place the HTML element's name in preceding the period which is in front of the class selector's name</a>
  </li>
  <li>
    <a>Here is the syntax of a CSS class selector that specifies which HTML elements should be affected:</a>

```c
p.className {
    propertyName: value;
    propertyName2: value2;
}
```
  <ul>
      <li>
        <a>In the class definition above, this class can now only be applied to the HTML element p</a>
      </li>
    </ul>
  </li>      
</ul>

### The CSS Universal Selector
<ul>
  <li>
    <a>The universal selector is denoted with a * which essentially selects all HTML elements within the code the CSS file is attached to</a>
  </li>
  <li>
    <a>Here is the syntax of a CSS universal selector:</a>

```css
* {
  propertyName: value;
  propertyName2: value2;
}
```
  </li>  
</ul>

### The CSS Grouping Selector
<ul>
  <li>
    <a>The grouping selector can be used when multiple HTML elements are desired to share the same class definitions</a>
  <li>
    <a>Here is the syntax of a CSS grouping selector:</a>

```css
htmlElement1, htmlElement2, htmlElement3 {
    propertyName: value;
    propertyName2: value2;
}
```
  </li>
  <li>
    <a>It is often better to use grouping selectors as a CSS class because it can help reduce the repetition of class definitions</a>
  </li>
</ul>    

## External, Internal, and Inline CSS
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
  </li>
  </ul>
  </li>
</ul>  

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
