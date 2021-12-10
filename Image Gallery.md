# Image Gallery

A picture is worth 1024 words. Today we will use HTML to make an image gallery.

## Images in HTML

The `<img>` tag is used to display images in HTML. When we want to show an image, we need to provide the **source** (`src`), which is the path to the image you want to show.

You can use an image on your own computer (or, if you're in an online coding environment, an image you upload), or you can use an image on the internet.

This is the syntax of the `<img>` tag (notice it **does not** have a closing tag):

```html
<img src="https://via.placeholder.com/300x75?text=Image%20Gallery">
```

<img src="https://via.placeholder.com/300x75?text=Image%20Gallery">

## Random Images

There are services in the software world called **APIs** (application programming interfaces), that can communicate certain data to other devices.

A fun one to play around with related to images is [Lorem Picsum](https://picsum.photos/), which provides random images for us. We can use these images in our HTML websites.

```html
<img src="https://picsum.photos/200/200">
```

<img src="https://picsum.photos/200/200">

## Reloading a page

If we are to display a random image onto the site everytime, we probably want a way for the user to reload the screen. There are *many* ways of reloading a page using HTML and JavaScript, but the one that's easiest for us right now, is below.

```html
<a href="index.html"></a>
```

This would work if the webpage you're making is under a file name of `index.html`. When the link is clicked, you will be brought to that page again, effectively reloading the page. If you named your HTML file something else, put that as the `href`.

Now, you have a website that presents a random image on load with a button to reload!

## Your turn!

It's your turn now. You can improve the website we made today, or you can learn something else on your own. One important skill that all good programmers need is learning things on their own.

It's no longer 1997, [Google](https://www.google.com/) exists! 😏
