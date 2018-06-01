# animated-cube-with-css3
How to animate a 3D Cube with just HTML and CSS3

Core skill: add animations to divs using css3 keyframes and transforms.

### Vendor specific commands for older browsers
When animations came around the first time, browser vendors needed to implement these commands in their particular browsers. At first we needed a prefix per vendor to make this work. For example:
	-webkit-perspective: 500px;
	-moz-perspective: 500px;
	-ms-perspective: 500px;
	-o-perspective: 500px;
	perspective: 500px;
At the top of the css file, the vendors for each prefix are listed.
Strangely enough (or perhaps predicatbly enough) Microsoft did not need a ms-prefix for the keyframes command. Actually, Microsoft Internet Explorer did not master CSS animations all that well after all...

### The HTML
For all intents and purposes the head section includes a viewport-tag, even though this demo is not responsive.

The outermost generic div holds a cube-wrapper which has two child elements: a text-div and the actual cube-div.
Inside this cube-div, there are six divs, representing the six individual sides of the cube.

There is not much more to it.

### The CSS
To get to a real cube, we need to give the scene (the cube-wrapper) some perspective first.

Next we will spin this 360 degrees on the vertical, or y-axis.
We call the animation and set the cube.
(This is where Internet Explorer has problems as preserve-3d does not seem to work)

Each individual side gets two css-stylings: a generic one applied to all sides and a specific one for each individual side.
This builds the planes that form the basic cube.

### Extra
As an added bonus the logo text is animated as well, just like a typewriter.

## [View the published result](https://vincentklijn.github.io/animated-cube-with-css3/) 
(This will work in most browsers, but IE will only show a flattened version of the spinning cube)
