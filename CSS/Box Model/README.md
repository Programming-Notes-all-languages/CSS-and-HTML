<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#the-box-model'>The Box Model</a>
  </li> 
  <li>
    <a href='#colors'>Colors</a>
  </li> 
  <li>
    <a href='#borders-margins-and-padding'>Borders, Margins, and Padding</a>
    <li>
    <a href='#outlines'>Outlines</a>
  </li> 
  </li> 
</ol>
</details>

## The Box Model
<ul>
  <li>
    <a>The box model states that every HTML element is wrapped within a CSS box. This box consists of: the content, padding, borders, and margins</a>
    <ul>
      <li>
        <a>The padding is transparent and serves as the buffer between the content and the border</a>
      </li>
      <li>
        <a>The border is the buffer between the padding and the margin. The border is not transparent</a>
      </li>
      <li>
        <a>The margin is the clear area on the outside of the border. The margin is also  transparent</a>
      </li>
    </ul>        
  </li>
</ul>   

![css-box-model](https://github.com/user-attachments/assets/4a73d686-2dad-477e-ae97-36761af5ad3b)

## Colors
<ul>
  <li>
    <a>To set the color of text, the color attribute can be used such as in the following: color: colorName;. The name of the color can be hex, rgb, hsl, or even just type the name of the color, if the color's name is already predefined</a>
  </li>
  <li>
    <a>The background color of a page too can be set using css. The syntax for setting the background color is the following: background-color: colorName;</a>
  </li>
  <li>
    <a>The opacity/transparency of an element can too be modified using css. The syntax for setting the opacity is the following: opacity: value; (where value ranges from 0.0 to 1.0)</a>  
</ul>    

## Borders, Margins, and Padding
### Borders
<ul>
  <li>
    <a>Here are a list of values that can be applied to the property border-style:</a>
    <ul>
      <li>
        <a>dotted: creates a dotted border</a>
      </li>  
      <li>
        <a>dashed: creates a dashed border</a>
      </li>
      <li>
        <a>solid: creates a solid border</a>
      </li>
      <li>
        <a>none: creates no border</a>
      </li>
      <li>
        <a>hidden: creates a hidden border</a>
      </li>
    </ul>
  </li>
  <li>
    <a>Border width can be manipulated by CSS' border</a>
    <ul>
      <li>
        <a>Here are examples of how to change an HTML element border's width</a>

```css
.border1 {
    border-style: solid;
    border-width: 1px /* 1px border on all sides */
}

.border2 {
    border-style: solid;
    border-width: 1px 20px /* 1px border top and bottom, 20px on left and right */
}
```
</li></ul></li>
  <li>
    <a>Border colors can be modified by CSS' border-color property</a>
    <ul>
      <li>
        <a>Here are examples of how to change to an HTML element border's color</a>  
        
```css
.border1 {
    border-style: solid;
    border-color: red /* changes border to red */
}

.border2 {
    border-style: solid;
    border-width: blue /* changes border to blue */
}
``` 
</li></ul></li>  
</ul>

### Margins
<ul>
  <li>
    <a>There are four margin properties that are used to alter the space that around HTML elements: margin-top, margin-right, margin-bottom, margin-left</a>
    <ul>
      <li>
        <a>The properties above can be set to equal a pixel length, such as 10px</a>
      </li>
    </ul>    
  </li>
</ul>

### Padding
<ul>
  <li>
    <a>Alike margins, there are four passing properties that are used to control the space that surrounds the HTML element's content: padding-top, padding-bottom, padding-right, and padding-left</a>
    <ul>
      <li>
        <a>The properties above can be set to equal a pixel length, such as 10px</a>
      </li>
    </ul>   
  </li>
</ul>    

## Outlines
<ul>
  <li>
    <a>Outlines are drawn outside of an HTML element's border. Outlines are often used to make an element stand out</a>
  </li>
  <li>
    <a>An outline is not part of the HTML element it surrounds</a>
  </li>
  <li>
    <a>An outline's color and width can be modified with outline-width and outline-color</a>
  </li>  
</ul>      