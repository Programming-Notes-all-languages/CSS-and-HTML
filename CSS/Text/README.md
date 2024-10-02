<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#text-alignment'>Text Alignment</a>
  </li> 
  <li>
    <a href='#fonts'>Fonts</a>
  </li>
  <li>
    <a href='#styling-links'>Styling Links</a>
  </li>
  <li>
    <a href='#list'>Lists</a>
  </li>  
  <li>
    <a href='#table'>Tables</a>
  </li>  
  <li>
    <a href='#position'>Position</a>
  </li>
  <li>
    <a href='#the-z-index-property'>The z index Property</a>
  </li>
  <li>
    <a href='#overflow'>Overflow</a>
  </li>
  <li>
    <a href='#the-float-property'>The float Property</a>
  </li>
</ol>
</details> 

## Text Alignment
<ul>
  <li>
    <a>The text-align property is used to change the horizontal alignment of a block of text</a>
  </li>
  <li>
    <a>There are four values for the text-align property: center (which centers the text), left (which left justifies the text) and right (which right justifies the text), and justify</a>
  </li>  
</ul>

## Fonts
<ul>
  <li>
    <a>The font-style property is used to change the appearance of a block of text</a>
    <ul>
      <li>
        <a>Here are some of the values for font-style: normal, italic, oblique</a>
      </li>
    </ul>
  </li>    
  <li>
    <a>The font-weight property is used to change the weight of a block of text</a>
    <ul>
      <li>
        <a>Here are some of the values for font-weight: normal and bold</a>
      </li>
    </ul>    
  </li>
  <li> 
    <a>The font-size property manipulates the size of text within an HTML element</a>
    <ul>
      <li>
        <a>Any value can be used to specify the size of the desired text</a>
      </li>
    </ul>
  </li>
  <li>
    <a>The font-family property is used to change the font of a block of text</a>
  </li>  
</ul>    

## Styling Links
<ul>
  <li>
    <a>There are four CSS properties that can be modified to change the appearance of a link under certain conditions</a>

```css
/* unvisited link */
a:link {
    color: red;
}

/* visited link */
a:visited {
    color: orange;
}

/* hovering over link */
a:hover {
    color: yellow;
}

/* selected link */
a:active {
    color: green;
}
```    
  </li>
  <li>
    <a>Here is a more advanced example of creating a link that appears to look like a button</a>

```html
<!DOCTYPE html>
    <html lang="en">
        <head>
            <meta charset="UTF-8"/>
            <title>My First Webpage</title>
            <link rel="stylesheet" href="style.css">
        </head>
        
        <!-- Header -->
        <header class="text">
            <h1>Link Button</h1>
            <p>Here is a link styled as a button:</p>
        </header>
        
        <!-- Body -->
        <body class="text">
            <span class="background">
                <a href="www.google.com" target="www.google.com"><strong>Click me!</strong></a>
            </span>
        </body>  
    </html>
```

```css
/* changes text font */
.text {
    font-family: "Times New Roman";
}

/* changes appearance of header */
header {
    color: #820025;
    background: rgb(247, 237, 218);
    padding: 0;
    margin: -8px;
    margin-top: -35px;
    font-size: 25px;
}

/* hovering over link */
a:hover {
    color: yellow;
}

/* visited link */
a:visited {
    color: purple;
}

/* selected link */
a:active {
    color: darkblue;
}

/* changes appearance of link */
.background {
    background-color: rgb(247, 237, 218);
    border-style: solid;
    border-color: rgb(247, 237, 218);
    border-width: 7px;
}
```
</li></ul>    

## Lists
<ul>
  <li>
    <a>In HTML, there are two different types of lists: ordered lists and unordered lists. Unordered lists are denoted with the ul tag and ordered lists are denoted with the ol tag</a>
  </li>
  <li>
    <a>The list-style-type property can be used to specify the type of list marker to denote each item of a list</a>
    <ul>
      <li>
        <a>Some values for this property are the following: circle, square, upper-roman, and lower-alpha</a>
      </li>
      <li>
        <a>Here is an example of using lists in CSS:</a>    
      
```html
<!DOCTYPE html>
    <html lang="en">
        <head>
            <meta charset="UTF-8"/>
            <title>My First Webpage</title>
            <link rel="stylesheet" href="style.css">
        </head>
        
        <!-- Body containing list -->
        <body>
            <ol class="background order">
                <li>
                    Coffee
                </li>
                <li>
                    Tea
                </li>
                <li>
                    Coca Cola
                </li>
            </ol>
        </body>  
    </html>
```    

```css
/* changes text font */
.text {
    font-family: "Times New Roman";
}

/* list type */
ol.order {
    list-style-type: upper-roman;
}

/* changes border surrounding list */
ol.background {
    border-color: lightcoral;
    border-width: 30px;
    padding: 0;
    width: 150px;
    border-style: solid;
    background: white;
}

/* changes text color */
li {
    color: darkred;
}
```
</li>
    </ul>    
  </li>  
</ul>

## Tables
<ul>
  <li>
    <a>To specify a table's border in CSS, the border property can be used</a>
  </li>
  <li>
    <a>The HTML tags used in creating a table, table, th, and td, can be altered using a class to create a table of any appearance</a>
  </li>
  <li>
    <a>The width property can be used to create a table of any width</a>
  </li>
  <li>
    <a>Similar to the width property, the height of a table can be altered too. This can be accomplished by modifying the height property within a CSS class</a>
  </li>
  <li>
    <a>The text-align property can be used to justify the elements within a table of any liking</a>
  </li>  
  <li>
    <a>The vertical-align property is used to change the alignment of the elements vertically</a>
    <ul>
      <li>
        <a>This property has three possible values: top, bottom, or middle</a>
      </li>
    </ul>
  </li>      
  <li>
    <a>When hovering over a table, the color of a row or column can be illuminated using the :hover property. Simply place either th, td or tr in front of :hover to highlight which row or column the cursor is hovering over. There are no special properties needed for this to be accomplished. Just choose the background color</a>
  </li>
  <li>
    <a>The property border-collapse is used to remove the individual borders of each element to form a single border between elements</a>
    <ul>
      <li>
        <a>To achieve the above, the value, collapse, can be assigned to this property</a>
      </li>
    </ul>
  </li> 

```html
<!DOCTYPE html>
    <html lang="en">
        <head>
            <meta charset="UTF-8"/>
            <title>My First Webpage</title>
            <link rel="stylesheet" href="style.css">
        </head>
        
        <!-- Table -->
        <table>
            <thead>
                <tr>
                    <th>First Name</th>
                    <th>Last Name</th>
                    <th>Age</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>John</td>
                    <td>Doe</td>
                    <td class="age">30</td>
                </tr>
                <tr>
                    <td>Jane</td>
                    <td>Smith</td>
                    <td class="age">28</td>
                </tr>
                <tr>
                    <td>Michael</td>
                    <td>Johnson</td>
                    <td class="age">40</td>
                </tr>
            </tbody>
        </table>
    </html>
```

```css
/* sets text font */
.text {
    font-family: "Times New Roman";
}

/* modifies table */
table {
    background-color: lightpink;
    border-collapse: collapse;
}

/* modifies thead and th */
thead th {
    border: solid;
    border-width: 1px;
    border-color: black;
}

/* modifies tbody and td */
tbody td {
    border: solid;
        border-width: 1px;
        border-color: black;
}

/* aligns age column */
td.age {
    text-align: center;
}

/* modifies header row's background color */
thead {
    background-color: palevioletred
}

/* changes element color when hovering */
td:hover {
    background-color: antiquewhite;
}
```
</ul>    

## Position
<ul>
  <li>
    <a>The position property is responsible for the position of HTML elements. There are five values that can be assigned to the position property</a>
  </li>
</ul>

<ul>
  <li>
    <a>For the remaining property values, the following additional properties can be used to position HTML elements on a webpage: top, bottom, left, and right</a>
  </li>
</ul>    

### Static
<ul>
  <li>
    <a>All HTML elements are static by default</a>
  </li>
  <li>
    <a>Elements with a position of static are not placed in any special way on a webpage</a>
  </li>
</ul>

### Relative
<ul>
  <li>
    <a>The relative value enables the HTML element to be moved relative to where the HTML element would be positioned if the position was set to static</a>
  </li>
</ul>    

### Absolute
<ul>
  <li>
    <a>HTML elements with a position of absolute are positioned relative to the nearest positioned ancestor, the nearest HTML element</a>
  </li>
</ul>    

### Fixed
<ul>
  <li>
    <a>The fixed value when applied to an HTML element keeps the element fixed on the screen, even when the page is scrolled</a>
  </li>
</ul>

### Sticky
<ul>
  <li>
    <a>The sticky value is a mix of relative and mix. The element sticks to the screen until the user scrolls down enough. Then, the element will stick to the screen at that point and for the remainder of the page. If the user scrolls back up, then the element will no longer stick</a>
  </li>
</ul>    

## The z-index Property
<ul>
  <li>
    <a>The z-index property specifies the precedence in which elements are stacked, whether one element should be in place above another or behind another</a>
  </li>
  <li>
    <a>The z-index property only works when the position is one of the following: absolute, relative, fixed, or sticky</a>
  </li>
  <li>
    <a>The z-index can be assigned an integer value. The lower the integer value, the less precedence, meaning that elements with higher z-indices will be on top of the elements with lower z-indices</a>
  </li>  
  <li>
    <a>Without z-indices, the elements defined last in the .html file will show up on top of the elements that appear earlier in the code</a>
  </li>  
</ul>    

## Overflow
<ul>
  <li>
    <a>Overflow in CSS specifies whether to add scroll bars or to clip the content within an element's box</a>
  </li>
</ul>    

### Visible
<ul>
  <li>
    <a>visible is the default value assigned to overflow. The overflow is not clipped and the content will appear outside of the element's box</a>
  </li>
</ul>   

### Hidden
<ul>
  <li>
    <a>When the overflow property is assigned to hidden, the content is clipped to fit within the element's box, but the rest of the content will be invisible</a>
  </li>
</ul>

### Scroll
<ul>
  <li>
    <a>The scroll value adds a scroll bar to the element's box and the information is clipped. Using the scroll bar, all the information can be viewed using the horizontal</a>
  </li>
</ul>    

### Auto
<ul>
  <li>
    <a>The value auto is similar to scroll, but it only adds the scroll bars when necessary</a>
  </li>
</ul>    

## The float Property
<ul>
  <li>
    <a>The float property is used to format text in a container with pictures</a>
  </li>
  <li>
    <a>The values that are associated with the property are: left, right, none and inherit</a>
    <ul> 
      <li>
        <a>none is the default value for float</a>
      </li>
      <li>
        <a>inherit is used to inherit the parent element's float value</a>
      </li>  
    </ul>
  </li> 
  <li>
    <a>When using the float property, the clear property will need to be used. The clear property specifies what should happen after the element that has a float property</a>
    <ul>
      <li>
        <a>The none element is the default value for clear</a>
      </li>
      <li>
        <a>The left value is used for HTML elements</a>
      </li>
    </ul>       
  </li>  
  <li>
    <a>If the float property is assigned a value of left, then the following HTML element should have a clear property that is assigned a value of left--if the intention of the next HTML block is to not be floated anymore</a>
  </li>  
  <li>
    <a>Sometimes, the content that is floated is taller than the picture, or in some instances, the text is larger than the image. In these cases, the clearfix property can be assigned to an HTML element to create a box that encompasses the largest element, leaving extra space around the smaller element</a>
    <ul>
      <li>
        <a>The value auto is often applied to the clearfix property</a>
      </li>
    </ul>    
  </li>  
</ul>    
