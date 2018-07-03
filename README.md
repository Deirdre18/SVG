## This is an SVG lesson (from Code Institute Full-Stack Diploma course). Transcription from lessons, included in comments sections in the code. 

# SVG Graphics

1. What is it?

Scalable Vector Graphics (SVG) is a standardised graphics rendering format based on XML.

2. What does it do?

An SVG allows for the creation of 2D graphics called Vector Graphics. Vector Graphics can be increased or decreased in size without loss of clarity.

3. How do you use it?

When creating Web based data visualisations you create SVGs just like you would ordinary HTML elements - mark up the elements in a web document and assign values to the element attributes

D3 and indeed most of data visualization tools are founded upon
what are called SVG's. So SVG stands for Scalable Vector Graphics. And SVG is a
family of specifications for creating vector graphics. Since vector graphics
are not created out of pixels they can be scaled up to larger or smaller sizes
without losing image quality .SVG images and their behaviors are defined in XML
format. Now remember XML is a superset of HTML
and the (Document Object Model)DOM includes XML as part of its specification. You can use the DOM tree
to access and update the structure content and the style of SVG images. Also
you can target SVG using Cascading Style sheets (CSS). As you can see on the screen you
create an SVG just as you would any other HTML element. So it has an opening
tag and a closing tag. Now the area in between the opening and closing tag is
called a viewport And in that viewport you can define child elements, which are
shapes such as rectangles, circles ellipses, polygons, paths, texts and
more. In our example we are creating a rectangle, and just like any other HTML
element it too has attributes - it has x and y coordinates which determine where
it's drawn on the screen it also has a width and a height. Also notice that by
default the color of the graphic will be black just like text rendered in black by default. Let's
define a circle now a circle has a C X and a C Y value which define the center
of the circle so it's x and y coordinate at the center you also define a radius
in our example we're setting our x value for the circle to be a hundred pixels
out from the left of the viewport and 25 pixels down from the top of the viewport
our radius is also equal to 20
let's change the color by adding a filter our rectangle and let's give it a
color red let's give the circle let's give this a color of blue render them
again and you can see that the circle overlays the rectangle that's because it
is rendered after the rectangle let's swap those around refresh the browser
and you can see that the rectangle now overlays the circle that's because the
rectangle appears after the circle in this case let's try another shape let's
try a polygon and a polygon relies on a number of points to map out its boundary
and by default all the points will be filled in to represent a solid shape
adding some points in here now remember in 2d graphics a point is made up of an
x-coordinate and a y-coordinate obviously in 3d graphics it's made of an
x-coordinate a y-coordinate and a z-coordinate or a Z coordinate here we can
see our polygons all the points are represented and there's a fill from the
origin of the Y and the x-axis out as far as they outermost point
let's play around with the rectangle again got it said its X&Y coordinates to
0 which means the top left-hand corner of our SVG viewport
unlike the plane that you would have learned in school the Cartesian plane
you had learned in school in computer graphics by default the origin is the
top left hand corner so we've defined a single rectangle let's copy and paste
this shape a few times and that's changed the x coordinate let's increase
it by 20 each time what we're going to do is create a series of bars moving
from left to right yes we rendered each bar is 20 pixels out further than the
last and each bar is only 19 pixels wide that's why you get to see the separators
now let's change the heights for these
save render bar chart or histogram but it's upside-down that's because in
computing the origin is on the top left-hand corner of the two-dimensional
plane but we can fix this and later when we get to d3 there are functions that
will do that automatically for us so that our bar charts appear the right way
up so what we're doing here is we're changing the y-coordinate so the
rendering will begin at different points on the y-axis moving down the screen and
there you get a more recognizable bar chart you can see here that this forms
the basics of data visualizations once we become familiar with the SVG we will
start working with data at the moment these values are hard-coded into each
rectangle object within the SVG viewport in later units we'll start working with
external data in order to provide that which is a much more realistic
representation of data visualizations and how they work but before we finish
let's change the color of each of these bars to make the differences and the
values stand out that little bit more so there you have it scalable vector
graphics use a viewport it's child elements are basic shapes and they can
be built upon and customized