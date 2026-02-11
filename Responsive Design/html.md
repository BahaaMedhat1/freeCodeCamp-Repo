# Basic HTMl.

## 1. Understanding HTML Attributes (Theroy).

### A- what Roles Does HTML Play on the Web?

- **HTML** :
  - Stands for Hyper Text Markup Langauges which used for building web pages
  - represents the content and structure of web page
    using Elements

- **Elements type** : opening and closing tag to put content between them
  self closing tag (void elements) and it doesn't have any content

- **Attribute**: special value that used to adjust behavoir of element

- **src**: Specifies the image location.
- **alt**: Provides short, descriptive text for an image.

### B- What Are Attributes and How Do They Work?

- **Attribute**: A value placed inside the opening tag or self-closing tag.  
  It provides additional information or controls how the element behaves.

- **Common Attributes**
  - **href**: Specifies the link URL.
  - **target**: Specifies where to open the link.

- **Boolean Attributes**
  - Do not require a value.
  - Used to specify the state of an element.
  - Examples: `checked`, `readonly`, `disabled`, `required`.

- **checked**: Specifies that a checkbox is checked by default.

---

## 2. Understanding The HTML Boilerplate (Theroy).

### A- What Is the Role of the Link Element in HTML, and How Can It Be Used to Link to External Stylesheets?

- **link**:
  - It's an Element used to link external resources (ex: stylesheets, icon, etc) with
    HTML Document.
  - It should be placed inside the head element
  - `rel Attribute`: used to specifiy the relationship between linked resources and HTML Document,
    In this situation, we need to specify that this linked resource is a stylesheet.

  ```html
  <link rel="stylesheet" href="./styles.css" />
  ```

  - `href Attribute`: used to specifiy the location of URL for the Linked Resource.

  - Another common use case for the link element is to link to icons. Here is an example of linking to a favicon, favicon is short for favorite icon

  ```html
  <link rel="icon" href="favicon.ico" />
  ```

### B- What Is an HTML Boilerplate, and Why Is It Important?

- **Boilerplate**:
  - It's like a ready-made template for web pages.
  - It's include the basic structure and essential elements every HTML Documents need.

  ```html
  <!DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="utf-8" />
      <meta name="viewport" content="width=device-width, initial-scale=1.0" />
      <title>freeCodeCamp</title>
      <link rel="stylesheet" href="./styles.css" />
    </head>
    <body></body>
  </html>
  ```

- **DOCTYPE declaration**:
  - It tells browsers which version of HTML you're using.
  ```html
  <!DOCTYPE html>
  ```
- **head section**:
  - It contain the site's meta data in `meta` elements (ex: character encoding, site's title, etc).

  ```html
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document Title Goes Here</title>
    <link rel="stylesheet" href="./styles.css" />
  </head>
  ```

- **body section**:
  - Its about page content.

  ```html
  <body>
    <h1>I am a main title</h1>
    <p>Example paragraph text</p>
  </body>
  ```

### C- What Is UTF-8 Character Encoding, and Why Is It Needed?

- **UTF-8 (UCS Transformation Format 8)**:
  - It is a standardized character encoding widely used on the web.
  - Character encoding is the method computers use to store characters as data.
  - UTF-8 supports every character in the Unicode character set - and this includes characters and symbols from all writing systems, languages, and technical symbols.

---

## 3. HTML Fundamentals (Theroy).

### A- What are Div Elements and When Should You Use Them?

- **div**:
  - It's an element that used as a container to group other elements.
  - We will mainly use the div element when we want to group HTML elements that will share a set of CSS styles.
- **section**:
  - It's an semantic element that has meaning over the div element which is not semantic.
  - It also used to group other elements that will share css styles.
  - `Semantics` are the meaning of words or phrases in a language

### B- What Are IDs and Classes, and When Should You Use Them?

- **id**:
  - It adds a unique identifier to an HTML element.
  - `The hash symbol (#)` tells the computer you want to target an id with that value.
  - id names should not be used more than once, and they should always be unique, and they cannot have spaces in them.

- **class**:
  - It's contrast of `id` attribute, and It doesn't need to be unique.
  - We use it when we want to apply a set of styles to many elements.
  - It can have spaces.

### C- What Are HTML Entities, and What Are Some Common Examples?

- **HTML Entity**:
  - `character reference,` is a set of characters used to represent a reserved character in HTML.

  - `named character references` starts with an ampersand sign (&) and end with a semicolon (;), etc: &amp; &lt; &gt; .

  - `decimal numeric reference` starts with an ampersand sign and hash symbol (#), followed by one or more decimal digits, followed by a semicolon, etc &#169; &#174; .

  - `hexadecimal numeric reference` starts with an ampersand sign, hash symbol, and the letter x. Then it is followed by one or more ASCII hex digits and ends with a semicolon, &#x20AC; &#x03A9;.

### D- What Is the Role of the Script Element in HTML, and How Can It Be Used to Link to External JavaScript Files?

- ## **script Element**:
  - is used to embed executable code in HTML document.

  ```html
  <script>
    // alert("Welcome to freeCodeCamp");?
  </script>
  ```

  - it is considered best practice to link to an external JavaScript file instead of writing inside HTML document to apply separate of concern principle.

  ```html
  <script src="path-to-javascript-file.js"></script>
  ```

  - `Separation of concerns` is a design principle where you separate your programs into distinct sections and have each section address a separate concern.

---
