# Painter

Today, we'll be learning about the p5.js library.

## p5.js

p5.js is a JavaScript library for creative coding. It can be used to create many fun programs, including in-browser games, graphics, and more.

## A basic p5.js program

Put this into your `script.js` file.

```js
function setup() {
  createCanvas(400, 400);
}

function draw() {
  background(200);
}
```

Here, you can see 2 functions: `setup()` and `draw()`.

`setup()` is responsible for setting up our environment. Right now, it creates a canvas that is 400 by 400.

`draw()` is called continuously after setup is complete. Right now, it repeatedly makes the background of our canvas gray.

Now let's change the program up a little bit. Add this line after `background(200);`

```js
rect(25, 25, 50, 50);
```

You should see a rectangle appear on your screen.

The `rect()` function takes the following parameters:

```js
rect(x, y, width, height);
```

Your turn: use the power of your search engine to find out how to draw a circle (ellipse).

The `ellipse()` function takes the following parameters:

```js
ellipse(x, y, width, height);  // same as rect!
```

Now let's get started on our painter. The main idea here is to continuously draw circles when the mouse is pressed, at the position of the mouse.

There are 3 variables that will be important in this program:

* `mouseIsPressed` tells us whether the mouse is pressed.
* `mouseX` is the x-position of the mouse
* `mouseY` is the y-position of the mouse

With these information in mind, try to write this program on your own. A possible solution is below.

```js
function setup() {
  createCanvas(400, 400);
  background(200);
}

function draw() {
  if (mouseIsPressed) {
    ellipse(mouseX, mouseY, 50, 50);
  }
}
```

Notice how the `background(200);` has been moved to the `setup()` function, since we only want to draw the background once instead of in every frame update.

The code above is not a perfect solution by any means, just a starting point. There are many things you can consider fixing...

* Removing the border (look into `noStroke()`)
* Changing the color of the drawing (look into `fill()`)
* Challenge: Making the drawing more continuous (consider changing the drawing from using ellipses to lines; look into `pmouseX` and `pmouseY`)
* Be creative!
