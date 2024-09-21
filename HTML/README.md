<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#start-of-html-pages'>Start of HTML Pages</a>
  </li> 
  <li>
    <a href='#structure-of-an-html-file'>Structure of an HTML File</a>
  </li> 
  <li>
    <a href='#the-anchor-tag'>The Anchor Tag</a>
  </li> 
  <li>
    <a href='#tables'>Tables</a>
  </li> 
  <li>
    <a href='#common-html-elements'>TCommon HTML Elements</a>
  </li> 
</ol>
</details>

## Start of HTML Pages
<ul>
  <li>
    <a>An HTML file must end with the .html extension. The home page of a site should be called index.html.</a>
  </li>  
  <li>
    <a>The first line in an HTML page is the HTML5 <em>doctype</em> declaration, which is the following: <a><</a>!doctype html<a>></a></a>
  </li>
  <li>
    <a>After the doctype, the HTML tag is then included. The lang attribute is also included to specify the language of the contents of the document</a>
    <ul>
      <li>
        <a>Here is the format of the HTML tag with the lang attribute: <a><</a>html lang="en"<a>></a></a>
      </li>
      <li>
        <a>The lang attribute for writing in english is "en", such as shown above</a>
      </li>  
    </ul>
  </li>  
  <li>
    <a>On the line after the HTML tag and the lang attribute comes the <a><</a>head<a>></a> tag</a>
  </li>
  <li>
    <a>The last essential tag is the following: <a><</a>meta charset="utf-8"<a>></a></a>    
    <ul>
      <li>
        <a>This tag is a void tag meaning it does not require a closing tag</a>
      </li>
      <li>
        <a>The value for charset should always be utf-8</a>
      </li>
    </ul>
  </li>           
</ul>    

## Structure of an HTML File
<ul>
  <li>
    <a>Here is the structure of a basic HTML file with some comments explaining the tags. (The syntax for comments is the following: <a><</a>!-- substance of comment --<a>></a>):</a>

```html
  <!doctype html>
  <html lang="en">
    <head>
      <meta charset="utf-8>
      <title>HTML Site</title>
    </head>
    <body>
      <!-- Headings -->
      <h1>Heading One</h1>
      <h2>Heading Two</h2>
      <h3>Heading Three</h3>
      <h4>Heading Four</h4>
      <h5>Heading Five</h5>
      <h6>Heading Six</h6>

      <!-- Paragraph -->
      <p>
        Lorem ipsum dolor sit amet, consectetur adip
      </p> 
      
      <!-- Lists -->
      <ul>
        <li>List item 1</li> 
        <li>List item 2</li> 
        <li>List item 3</li> 
        <li>List item 4</li> 
      </ul>  
      
      <ol>
        <li>List item 1</li> 
        <li>List item 2</li> 
        <li>List item 3</li> 
        <li>List item 4</li>
      </ol>        
    </body>  
  </html>  
```  
  </li>
</ul>  

## The Anchor Tag
<ul>
  <li>
    <a>The anchor tag is used to link the document that the user is viewing to another document on a different location on the internet</a>
  </li>
  <li>
    <a>The anchor tag has the following syntax: <a><</a>a href="websiteName"<a>></a>text that will be linked to send user to other document<a><</a>/a<a>></a></a>
    <ul>
      <li>
        <a>What the above does it when the user clicks on the anchor tag, the current page that the user is viewing closes and is replaced with the page linked to the anchor tag</a>
      </li>
      <li>
        <a>To prevent the anchor tag from replacing the current website that the user is viewing, the following can be done: <a><</a>a href="websiteName" target="websiteName"<a>></a>text that will be linked to send user to other document<a><</a>/a<a>></a></a>
      </li>
      <li>
        <a>The target tag attribute will open up a new page so that the user can view either the linked page or the current page. This is often not useful when navigating on a single site; however, it is extremely useful when navigating to a different website</a> 
      </li>  
    </ul>
  </li>      
</ul>    

## Tables
<ul>
  <li> 
    <a>Here is the syntax for creating a table:</a>  

```html
  <!doctype html>
  <html lang="en">
    <head>
      <meta charset="utf-8>
      <title>HTML Site</title>
    </head>
    
    <!-- Table -->
    <table>
      <thead>
        <tr>
          <th>Name</th>
          <th>Email</th>
          <th>Age</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Garrett Ellis<td>
          <td>egarrett@gmail.com</td>
          <td>21</td>
        </tr>
      </tbody>
    </table>             
  </html>  
```  
  </li>
</ul>  

## Common HTML Elements
<ul>
  <li>
    <a>The <a><</a>div<a>></a> element is used to divide things into sections. This tag is often a last resort when the coder is unsure of how to proceed with sectioning off information</a>
  </li>
  <li>
    <a>The <a><</a>p<a>></a> element is used to mark up text of any length. This element is often a better choice than div</a>
  </li>
  <li>
    <a>The <a><</a>details<a>></a> and <a><</a>summary<a>></a> elements are used to create a widget that can open and close on a page. There is a piece of text written in the summary that when clicked, will display the contents of the widget</a>
  </li>
  <li>
    <a>Here is an example of these two elements in action:</a>

```html
  <!doctype html>
  <html lang="en">
    <head>
      <meta charset="utf-8>
      <title>HTML Site</title>
    </head>
    
    <details>
      <summary>Click me!</summary>
      <p>
        I have been revealed!
      </p>
    </details>
  </html>  
```
  </li>
  <ul>
    <li>
      <a>The <a><</a>strong<a>></a> element makes the encapsulated text within the tags bold</a>
    </li>   
    </li>
    <li>
      <a>The <a><</a>em<a>></a> element italicizes the encapsulated text within the tags</a>
    </li>
    <li>
      <a>The a><</a>span<a>></a> is equivalent to the div element. It is very useful for styling purposes</a>
    </li>  
  </ul>  
</ul> 

## Forms
<ul>
  <li> 
    <a>Here is some code illustrating how to use tags associated with creating forms:</a>

```html
  <!doctype html>
  <html lang="en">
    <head>
      <meta charset="utf-8>
      <title>HTML Site</title>
    </head>
    
    <!-- Forms -->
    <form action="process.php" method="POST">
      <span>
        <label>First Name</label>
        <input type="text" name="firstName"> 
      </span>
      <span>
        <label>Last Name</label>
        <input type="text" name="lastName">
      </span>  
    </form>    
  </html>  
```  
  </li>
</ul>  

## Images
<ul>
  <li>
    <a>Here is some code showing how to display an image with HTML tags:</a>
    
```html
  <!doctype html>
  <html lang="en">
    <head>
      <meta charset="utf-8>
      <title>HTML Site</title>
    </head>
    
    <!-- Images -->
    <img src="Images/Horizon.jpg" alt="Carnival Horizon">   
  </html>  
```
  </li>
  <li>
    <a>The anchor tag can actually be used to open up an image to have it open on a new/different tab. This can be done by encapsulating the img tag within the anchor tag such as in the following example:</a>

```html
  <!doctype html>
  <html lang="en">
    <head>
      <meta charset="utf-8>
      <title>HTML Site</title>
    </head>
    
    <!-- Images -->
    <a href="Images/Horizon.jpg">
      <img src="images/Horizon.jpg" alt="Carnival Horizon">
    </a>    
  </html>  
```
  </li>
</ul>  