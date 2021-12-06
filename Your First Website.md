# Your First Website

Today, you will learn about HTML and use it to make your first website.

## HTML

Let's first talk a little bit about HTML. HTML stands for **HyperText Markup Language**, and is the standard markup language used to create websites.

The super majority of the websites you use everyday are all powered by HTML. If you go to your favorite site, and press `CTRL+SHIFT+I` (or right click and click inspect in the pop-up menu), you will see the HTML document that renders the web page!

When you go to a website, the server of that website sends the HTML code (in addition to other documents which we need not worry about at this moment) of the website to your web browser (example: Google Chrome), which renders it.

### HTML Elements

HTML is made up of **elements**. Different HTML elements are rendered differently by the web browser.

An HTML element looks something like this:

```html
<tag-name>Content</tag-name>
```

Notice how the element starts with a **start tag**, which tells the browser that an element is starting. Then there is the **content** of the tag, which is usually the text that will be displayed. After that is an **end tag** (note the forward slash before the `tag-name`).

*Note: Some elements do not have content or an end tag*

#### Heading elements

HTML heading elements are titles/subtitles.

HTML has the heading tags `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>`, `<h6>`. `<h1>` is the biggest, and `<h6>` is the smallest.

```html
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
```

will be displayed as...

<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>

#### Paragraphs

The `<p>` tag tells browsers to display text as paragraphs.

```html
<p>Here is a paragraph</p>
<p>And another one here.</p>
```

<p>Here is a paragraph</p>
<p>And another one here.</p>

#### Links

Links are very useful. Users can click on links to go to another site.

In HTML, `<a>` defines a hyperlink, and follows the following format.

```html
<a href="url">Text</a>
```

Here's an example:

```html
<a href="https://youtu.be/dQw4w9WgXcQ">Here's an example link 😇</a>
```

<a href="https://youtu.be/dQw4w9WgXcQ">Here's an example link 😇</a>

### HTML documents

HTML documents follow some rules so web browsers properly display the code they contain. Below is a boilerplate template for a basic HTML document.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Title of the Page</title>
  </head>

  <body>
    <!-- Body of your HTML document -->
  </body>
</html>
```

The `<!DOCTYPE html>` tag is telling browsers the document type of HTML is present. It does not have a closing tag and appears at the very top of HTML documents.

The `<head>` element contains metadata about the HTML document. Don't worry about these for now, besides the `<title>` tag, which contains the title shown in the browser's tab.

Then there's the `<body>` tag, which contains all the content of the website, like text, images, links, videos, etc.

Here's an example website made with the simple elements discussed above.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About Python</title>
  </head>

  <body>
    <h1>About Python - a simple introduction to a not-so-simple programming language</h1>

    <h2>Overview</h2>
    <p>Python is an interpreted high-level general-purpose programming language. Its design philosophy emphasizes code readability with its use of significant indentation. Its language constructs as well as its object-oriented approach aim to help programmers write clear, logical code for small and large-scale projects. <a href="https://en.wikipedia.org/wiki/Python_(programming_language)">Wikipedia</a></p>

    <h2>Name</h2>
    <p>Python is called "Python", spelled with the following letters of the English lexicon: "p". "y", "t", "h", "o", and "n".</p>

    <h2>Some useful links related to Python:</h2>
    <p><a href="https://www.python.org/">Python.org</a></p>
    <p><a href="https://www.python.org/psf/">Python Software Foundation</a></p>
    <p><a href="https://youtu.be/dQw4w9WgXcQ">Totally Legit Python Website</a></p>

  </body>
</html>
```

Now, your turn! Make a simple website about something you're interested in, whether it's a sport, a book you've read recently, or your favorite traveling destination.
