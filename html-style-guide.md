# HTML Style Guide
## Table of Contents

1. [General HTML Formatting](#general-html-formatting)
2. [Always close elements](#always-close-elements)
3. [Capitalization](#capitalization)
4. [Doctype](#doctype)
5. [HTML Quotation Marks](#html-quotation-marks)
6. [Including Stylesheets and Scripts](#including-stylesheets-and-scripts)
7. [Indentation](#indentation)

## General HTML Formatting

- [1.1](#1.1) Paragraphs of text should always be placed in a <code>&lt;p&gt;</code> tag. Never use multiple <code>&lt;br&gt;</code> tags.

  ```html
        <p>My precious!</p>
  ```
- [1.2](#1.2) Items in list form should always be in <code>&lt;ul&gt;</code>, <code>&lt;ol&gt;</code>, or <code>&lt;dl&gt;</code>. Never use a set of <code * s="typ">&lt;div&gt;</code> or <code>&lt;p&gt;</code>.

  ```html
        <ul>
            <li>Gandalf</li>
            <li>Aragorn</li>
            <li>Frodo</li>
            <li>Gimli</li>
        </ul>
    ```
- [1.3](#1.3) Every form input that has text attached should utilize a <code >&lt;label&gt;</code> tag. <strong>Especially radio or checkbox elements.</strong>

    ```html
        <label for="my-input">Enter Rivendell</label>
        <input type="radio" class="this-class" name="my-input">
    ```
    
- [1.4](#1.4) Even though quotes around attributes is optional, always put quotes around attributes for readability.

    ```html
        <img src="images/saruman.jpg" alt="White Wizard">
    ```
    
- [1.5](#1.5) Avoid trailing slashes in self-closing elements.

    ```html
        <br> 
        <hr> 
        <img>
        <input>
    ```

- [1.6](#1.6) Use a new line for every block, list, or table element, and indent every such child element.
  
   ```html
       <table>
          <thead>
                <tr>
                    <th>Dwarf</th>
                    <th>Elf</td>
                </tr>
          </thead>
          <tbody>
                <tr>
                    <td>Gimli</td>
                    <td>Legolas</td>
                </tr>
          <tbody>
       </table>
   ```
   
## Always Close Elements
Don’t omit optional closing element tags.
   ```html
    <p>Always use closing tags.</p>
   ```
   
## Capitalization
All code has to be lowercase: This applies to HTML element names, attributes, attribute values (unless text/CDATA), CSS selectors, properties, and property values (with the exception of strings).</p>
   ```html
    <label for="my-input">TreeBeard</label>
    <input class="this-class" name="my-input">
   ```
   
## Doctype
Always use the HTML5 doctype. HTML5 (HTML syntax) is preferred for all HTML documents.
   ```html
    <!Doctype html>
   ```

## HTML Quotation Marks
When quoting attributes values, use double quotation marks.
   ```html
    <img src="images/gandalf.jpg" alt="Gandalf"> 
    <h1 class="secret-safe">Is it secret? Is it safe?</h1>
```
## Including Stylesheets and Scripts
Use simple syntax for linking style sheets and scripts. The <code class="typ">type</code> attribute for style sheets and scripts is unnecessary.
   ```html
   <link href="style.css" rel="stylesheet">
   <script src="my-script.js"></script>
```
## Indentation
Indent by 4 spaces at a time. Don't use tabs (unless you set the 'indent using spaces' or 'soft indent' setting for your code editor).
   ```html
   <ul>
      <li>Faramir</li>
      <li>Bor0mir</li>
   </ul> 
```
