<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#combinators'>Combinators</a>
  </li> 
</ol>
</details> 

## Combinators
### Descendant Selector
<ul>
  <li>
    <a>The descendent selector is denoted by at lease one space character where HTML elements are spearated by spaces</a>
  </li>
  <li>
    <a>Here is the syntax for a descendant combinator:</a>

```css
htmlElement1 htmlElement2 {
    property1: value1;
    property2: value2;
}
```
  <ul>
      <li>
        <a>In the definition above, the properties of this class will applie to all htmlElement2s that are embedded within htmlElement1</a>
      </li>
      <li>
        <a>htmlElement2 can be embedded within another HTML element that too is embedded within htmlElement1. In this instances, the properties defined in the class will still apply to htmlElement2</a>
      <li>
    </ul>      
  <li>
</ul>    

### Child Selector
<ul>
  <li>
    <a>The child selector is denoted with the greater than character on the keyboard, >, and operates very similarly to the descendant selector</a>
  </li>
  <li>
    <a>Here is the syntax for the child slecetor:</a>

```css
htmlElement1 > htmlElement2 {
    property1: value1;
    property2: value2;
}
```
  <ul>
      <li>
        <a>The child HTML element, htmlElement2 in the definition above, must directly be one level of nesting underneath the parent HTML element, htmlElement1; otherwise, the proeprties defined within the class will not apply to htmlElement2</a>
      </li>
    </ul>
  </li>
</ul> 

### Adjacent Sibling Selector
<ul>
  <li>
    <a>
