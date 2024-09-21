![css-box-model](https://github.com/user-attachments/assets/4a73d686-2dad-477e-ae97-36761af5ad3b)
<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#start-of-html-pages'>Start of HTML Pages</a>
  </li> 
  <li>
    <a href='#the-anchor-tag'>The Anchor Tag</a>
  </li> 
</ol>
</details>

## Linking an .html file to a .css file
<ul>
  <li>
    <a>To get the content within the css file to apply to the html file, the following line of code can be used: <a><</a>link rel="stylesheet" href="filePath.css"<a>></a></a>
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
    <a>If a class is named with a string that is different than any html tag, the class' attributes can still be reflected within the html file</a>
    <ul>
      <li>
        <a>For instance, if a class has the following declaration:

```html
.gray {
color: gray;
}
```

then any section of the code within the html file can obtain the attributes defined within the class. This is accomplished by proceeding the name of the tag within the arrow with the following: <a><</a>tagName class="className"<a>></a>. This is only needed in the opening tag--not in the closing tag</a>
      </li>
    </ul>
  </li>  
  <li>
    <a>The name of a class in css starts with a period (.) if the class name is not an HTML tag; otherwise, the class name does not start with a period</a>
  </li>         
</ul>    

## The Box Model
<ul>
  <li>
    ![Here]([https://github.com/user-attachments/assets/3d7537a3-e7ec-4bf0-8661-0872112d3374](https://github.com/Programming-Notes-all-languages/CSS-and-HTML/blob/main/CSS/Selectors/Images/css-box-model.png](https://github.com/Programming-Notes-all-languages/CSS-and-HTML/blob/main/CSS/Selectors/Images/css-box-model.png))
)
