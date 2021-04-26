<img src ="https://cms-assets.tutsplus.com/uploads/users/1251/posts/28278/preview_image/chartjs-tutsplus.jpg">

#  **Chart.js**

Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.

A great way to get started with charts is with Chart.js, a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. It’s a well documented plugin that makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy.

## Installation

You can get the latest version of Chart.js from npm , the GitHub releases , or use a Chart.js CDN . Detailed installation instructions can be found on the installation page.

## Setting up

The first thing we need to do is download Chart.js. Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in. Then create a new html page and import the script,then :

1. Drawing a line chart
2. Drawing a pie chart
3. Drawing a bar chart

## 3.x Migration Guide

Chart.js 3.0 introduces a number of breaking changes. Chart.js 2.0 was released in April 2016. In the years since then, as Chart.js has grown in popularity and feature set, we've learned some lessons about how to better create a charting library. In order to improve performance, offer new features, and improve maintainability, it was necessary to break backwards compatibility, but we aimed to do so only when worth the benefit. Some major highlights of v3 include:

* Large performance improvements including the ability to skip data parsing and render charts in parallel via webworkers 

* Additional configurability and scriptable options with better defaults

* Completely rewritten animation system

* Rewritten filler plugin with numerous bug fixes

* Documentation migrated from GitBook to Vuepress

* API documentation generated and verified by TypeDoc

* No more CSS injection

* Tons of bug fixes

* Tree shaking


## Data structures

The data property of a dataset can be passed in various formats. By default, that data is parsed using the associated chart type and scales.

If the labels property of the main data property is used, it has to contain the same amount of elements as the dataset with the most values. These labels are used to label the index axis (default x axes). The values for the labels have to be provided in an array. The provides labels can be of the type string or number to be rendered correctly. In case you want multiline labels you can provide an array with each line as one entry in the array.

## Accessibility

Chart.js charts are rendered on user provided canvas elements. Thus, it is up to the user to create the canvas element in a way that is accessible. The canvas element has support in all browsers and will render on screen but the canvas content will not be accessible to screen readers.

With canvas, the accessibility has to be added with ARIA attributes on the canvas element or added using internal fallback content placed within the opening and closing canvas tags.

## Chart types :

<img src ="https://design.gccollab.ca/static/line_graph-6a065d6bb900f363e5dec8ac3d09ffb5-29ce1.png">

* **Line Chart**

A line chart is a way of plotting data points on a line. Often, it is used to show trend data, or the comparison of two data sets.

<img src = "https://www.xara.com/wp-content/uploads/2020/09/uncategorized-11341.jpg">

* **Bar Chart**

A bar chart provides a way of showing data values represented as vertical bars. It is sometimes used to show trend data, and the comparison of multiple data sets side by side.

<img src ="https://miro.medium.com/max/389/1*sLZFwG4PXJwpD0A_d90Fhg.png">

* **Doughnut and Pie Charts**

Pie and doughnut charts are probably the most commonly used charts. They are divided into segments, the arc of each segment shows the proportional value of each piece of data.

They are excellent at showing the relational proportions between data.

Pie and doughnut charts are effectively the same class in Chart.js, but have one different default value - their cutout. This equates to what portion of the inner should be cut out. This defaults to 0 for pie charts, and '50%' for doughnuts.

They are also registered under two aliases in the Chart core. Other than their different default value, and different alias, they are exactly the same.

<img src ="https://img.presentationload.com/webp/D0931/Radar-Charts_D0931_003_16x9_xl.webp">

* **Radar Chart**
A radar chart is a way of showing multiple data points and the variation between them.

They are often useful for comparing the points of two or more different data sets.

<img src ="https://i.pinimg.com/originals/7b/5b/f5/7b5bf575d5bacbfec5738985703b3525.jpg">

* **Polar Area Chart**

Polar area charts are similar to pie charts, but each segment has the same angle - the radius of the segment differs depending on the value.

This type of chart is often useful when we want to show a comparison data similar to a pie chart, but also show a scale of values for context.


<img src ="https://apexcharts.com/wp-content/uploads/2018/05/simple-bubble-chart.svg">

* **Bubble Chart**

A bubble chart is used to display three dimensions of data at the same time. The location of the bubble is determined by the first two dimensions and the corresponding horizontal and vertical axes. The third dimension is represented by the size of the individual bubbles.


<img src = "https://doc-archives.microstrategy.com/producthelp/10.6/AdvancedReportingGuide/WebHelp/Lang_1033/Content/AdvancedReporting/Graphics/GraphScatterXY2.png">

* **Scatter Chart**

Scatter charts are based on basic line charts with the x axis changed to a linear axis. To use a scatter chart, data must be passed as objects containing X and Y properties. The example below creates a scatter chart with 4 points.


# **Basic usage of canvas**

## The canvas element

At first sight a canvas looks like the img element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the canvas element has only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS, but during rendering the image is scaled to fit its layout size: if the CSS sizing doesn't respect the ratio of the initial canvas, it will appear distorted.

he canvas element differs from an img tag in that, like for video, audio, or picture elements, it is easy to define some fallback content, to be displayed in older browsers not supporting it, like versions of Internet Explorer earlier than version 9 or textual browsers. You should always provide fallback content to be displayed by those browsers.

Providing fallback content is very straightforward: just insert the alternate content inside the canvas element. Browsers that don't support canvas will ignore the container and render the fallback content inside it. Browsers that do support canvas will ignore the content inside the container, and just render the canvas normally.


# **Drawing shapes with canvas**

## The grid

Before we can start drawing, we need to talk about the canvas grid or coordinate space. Our HTML skeleton from the previous page had a canvas element 150 pixels wide and 150 pixels high. To the right, you see this canvas with the default grid overlayed. Normally 1 unit in the grid corresponds to 1 pixel on the canvas. The origin of this grid is positioned in the top left corner at coordinate (0,0). All elements are placed relative to this origin. So the position of the top left corner of the blue square becomes x pixels from the left and y pixels from the top, at coordinate (x,y). Later in this tutorial we'll see how we can translate the origin to a different position, rotate the grid and even scale it, but for now we'll stick to the default.

## Drawing paths

Now let's look at paths. A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color. A path, or even a subpath, can be closed. To make shapes using paths, we take some extra steps:

First, you create the path.
Then you use drawing commands to draw into the path.
Once the path has been created, you can stroke or fill the path to render it.
Here are the functions used to perform these steps:

**beginPath()**

Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
Path methods
Methods to set different paths for objects.

**closePath()**

Adds a straight line to the path, going to the start of the current sub-path.

**stroke()**

Draws the shape by stroking its outline.

**fill()**

Draws a solid shape by filling the path's content area.
The first step to create a path is to call the beginPath(). Internally, paths are stored as a list of sub-paths (lines, arcs, etc) which together form a shape. Every time this method is called, the list is reset and we can start drawing new shapes.

# **Applying styles and colors**

## Colors

Up until now we have only seen methods of the drawing context. If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.

* fillStyle = color

Sets the style used when filling shapes.

* strokeStyle = color

Sets the style for shapes' outlines.
color is a string representing a CSS color, a gradient object, or a pattern object. We'll look at gradient and pattern objects later. By default, the stroke and fill color are set to black (CSS color value #000000).

## Line styles

There are several properties which allow us to style lines.

lineWidth = value

Sets the width of lines drawn in the future.

lineCap = type

Sets the appearance of the ends of lines.

lineJoin = type

Sets the appearance of the "corners" where lines meet.

miterLimit = value

Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.

getLineDash()

Returns the current line dash pattern array containing an even number of non-negative numbers.

setLineDash(segments)

Sets the current line dash pattern.

lineDashOffset = value

Specifies where to start a dash array on a line.

# **Drawing text**

The canvas rendering context provides two methods to render text:

fillText(text, x, y [, maxWidth])

Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.

strokeText(text, x, y [, maxWidth])

Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

## Styling text

In the examples above we are already making use of the font property to make the text a bit larger than the default size. There are some more properties which let you adjust the way the text gets displayed on the canvas:

font = value

The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.

textAlign = value

Text alignment setting. Possible values: start, end, left, right or center. The default value is start.

textBaseline = value

Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.

direction = value

Directionality. Possible values: ltr, rtl, inherit. The default value is inherit.

# THE END