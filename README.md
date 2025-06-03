# vibe_coding_test

This repository contains a simple p5.js example. The `index.html` file loads
p5.js from a CDN and renders a bouncing 3D sphere on a 600 × 400 canvas.

## Running the demo

Open `index.html` in a modern web browser. The page will display a black
background with a sphere moving around the canvas. The sphere bounces off the
edges of the canvas and its colour can be changed by clicking anywhere on the
page.

## How it works

The animation is implemented in a small script included inside `index.html`.
When the page loads, `setup()` creates the canvas in `WEBGL` mode and adds one
ball using `addBall()`. Each frame, the `draw()` function updates the ball’s
position, checks for collisions with the canvas boundaries and renders the
sphere.

A click triggers `mousePressed()`, which picks a random ball (currently there is
only one) and assigns it a random colour. The code includes an `addBall()`
helper that can be used to push additional balls to the `balls` array if you
wish to extend the example.

