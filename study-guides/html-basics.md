# HTML Basics

**The HTML file is the most important file when building a basic website.** Some online IDEs like [Glitch](https://glitch.com/) or [Replit](https://replit.com/), you may notice that a basic website project comes pre-loaded with at least 3 files with the names `index.html`, `style.css`, and `script.js`. These are typical generic names an HTML, CSS, and JavaScript file, but you can name your files any name you want. It is always best practice to give your files a short descriptive name so that it is easier for others to view your code.

All websites **must have at least one HTML file**, but CSS style and JavaScript script files are **optional**. To learn more about file naming conventions and organization tips, check out [MDN web docs on dealing with files](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/Dealing_with_files).

*Note:* Web servers will often default to loading the `index.html` file if multiple HTML files are present, unless otherwise specified.
html is the skeleton of a website basically
## What is HTML?

**HTML** stands for **H**yper **T**ext **M**arkup **L**anguage. HTML is used to build the skeleton of the website including which elements (text, images, buttons, etc.) should be included and the order in which they appear. Web browsers like Chrome or Safari know how to interpret HTML files and render their contents as an interactive web page.

To collect all of this information, we use the `input` element and specify the type of information by using the `type` attribute.

Let’s take a look at a few examples of how the `input` element is used for a variety of types of information.

<<<<<<< HEAD
**Note:** The `form` element itself sets up an area to collect user input but does nothing with the information. This is where JavaScript steps in to process the data and make appropriate actions. This is why it is important to give each element an `id`, `name`, and/or `class`.
=======
**Let’s take a look at a typical boilerplate, or standard template, for an HTML file.**

```html
<!DOCTYPE html>
<html>
 <head>
   <meta charset="utf-8">
   <meta name="viewport" content="width=device-width">
   <title>Title of Website</title>
   <link href="style.css" rel="stylesheet" type="text/css" />
 </head>
 <body>
   <script src="script.js"></script>
 </body>
</html>
```

In HTML, we denote an element by specifying the name of the element in opening brackets `<>` and closing brackets `</>`. Let’s take the time to highlight the structure of an HTML file and some important elements presented in the boilerplate above.

- `<!DOCTYPE html>`: This specifies the document type and lets the computer know that we will be working in HTML. Most specifically our document will default to HTML5, which is the most recent major HTML version, unless otherwise specified.
- `<html>`: This is where we place all of our elements that comprise the contents of our page.
- `<head>`: This is the container for the elements that have content that does not need to be displayed on the page (like metadata, the title, or, as we will see, scripts and stylesheets).
- `<meta>`: This is a tag for providing metadata (data about our data) to the page. We can use meta tags to display what character set we are using or for SEO (Search Engine Optimization) purposes.
- `<title>`: This tag gives the page a title that can be displayed in the tab of your browser.
- `<body>`: This defines the main content of the HTML page.
### Linking JavaScript Files

**Line 9**  `<script src="script.js"></script>` links the JavaScript file to our HTML file.

Let’s break down the syntax used to do this action.

- `<script>`: You may be wondering, why do we use the `script` element to connect JavaScript files instead of the `link` element that is used for CSS files. Unlike CSS styling, JavaScript dynamically changes elements in the HTML document. JavaScript may add, delete, or modify HTML elements. CSS styling can only change the appearance of an element, but cannot modify the structure of the HTML element.
- `src`: This attribute specifies the file path, or location, of our external resource. In this particular example, the JS file is named `script.js` but you can name your stylesheet anything. Take note that the file path is surrounded by double quotes, `“”`.

You may have noticed that the `<script>` element is placed inside of the `<body>` element. This is different from the `<link>` element for CSS files which is in the `<head>` element. This is because JavaScript files can often affect the HTML elements within the document. To ensure that the JavaScript file does not run before the HTML elements have been loaded on the page, developers tend to place the `<script>` element towards the bottom of the HTML file to avoid potential errors.
>>>>>>> 0ed8492e9e73ff352f1efb1a0d973868cbe979d7
