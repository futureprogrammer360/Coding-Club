# Stylish Pages

So far, the websites we have created have all only included HTML, which defines the content of sites (the information that will show up). Today, we'll learn about CSS, which allows us to add style to our webpages.

## CSS

CSS stands for **Cascading Style Sheets**, and is a style sheet language whose sole purpose is to style HTML documents. We use CSS to describe how HTML elements should be displayed. CSS can style elements' colors, layouts, positions, and more.

CSS code can either live in-line in HTML, or in separate CSS files. Today we're going to focus on using CSS in their own files.

CSS uses rules to style elements. Each rule is made up of a **selector** and **declaration(s)**.

```css
h1 {
  color: red;
  text-align: center;
}
```

In the example above, we use CSS to style all `h1` elements to have the color red and be centered. `h1` is the selector. Following the selector inside of curly brackets are the declarations. Right now we have two: `color: red` and `text-align: center`. Notice how a semicolon ends each declaration.

So now, all the `h1` elements in my webpage will be red and centered (unless otherwise overridden by other CSS rules).

```html
<h1>Red and Centered</h1>
```

### Other CSS selectors

We can use a tag selector to style all elements with that tag. We can also be more specific when selecting elements.

#### Selecting by `class`es

One way to be more specific when selecting elements to style is using HTML `class`es.

If our HTML element looks like this...

```html
<p class="blue">Blue</p>
```

We can style elements with `class` `blue` with the following rule.

```css
.blue {
  color: blue;
}
```

#### Selecting by `id`s

If we want to be even more specific, we can select elements using `id`s.

```html
<p id="first-p">First paragraph</p>
```

```css
#first-p {
  text-decoration: underline;
}
```

The information above is barely scratching the surface of what CSS can do. CSS can style much more than just colors and text styles. When starting off with using CSS, feel free to just search up "How to change font family in CSS?" and learn as you code. The answer is the `font-family` property by the way.

Now it's your turn. Style one or a few of the HTML sites you created previously.
