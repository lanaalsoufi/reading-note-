# **Chapter (16)**

# IMAGES


## CONTROLLING SIZES OF IMAGES IN CSS 

You can control the size of an image using the width and height properties in CSS, just like you can for any other box.

Specifying image sizes helps pages to load more smoothly because the HTML and CSS code will often load before the images, and telling the browser how much space to leave for an image allows it to render the rest of the page without waiting for the image to download.

You might think that your site is likely to have images of all different sizes, but a lot of sites use the same sized image across many of their pages.

## AligNing images Using CSS

*The float property can be used to move an element to the left or the right of its containing block allowing text to flow around it. 

Rather than using the (img) element's align attribute, web page authors are increasingly using the float property to align images. There are two ways that this is commonly achieved:

1. The float property is added to the class that was created to represent the size of the image (such as the small class in our example).

2. New classes are created with names such as align-left or align-right to align the images to the left or right of the page. These class names are used in addition to classes that indicate the size of the image.

## Centering images Using CSS

By default, images are inline elements. This means that they flow within the surrounding text. In order to center an image, it should be turned into a blocklevel element using the display property with a value of block.

Once it has been made into a block-level element, there are two common ways in which you can horizontally center an image:

1. On the containing element, you can use the text-align property with a value of center.

2. On the image itself, you can use the use the margin property and set the values of the left and right margins to auto.

You can specify class names that allow any element to be centered, in the same way that you can for the dimensions or alignment of images.

## Background Images 

The background-image property allows you to place an image behind any HTML element. This could be the entire page or just part of the page. By default, a background image will repeat to fill the entire box.

The path to the image follows the letters url, and it is put inside parentheses and quotes.

## Repeating Images background-repeat background-attachment

The background-repeat
property can have four values:

***repeat***

The background image is repeated both horizontally and vertically (the default way it is shown if the backgroundrepeat
property isn't used).

***repeat-x***

The image is repeated horizontally only (as shown in the first example on the left).

***repeat-y***

The image is repeated vertically
only.

***no-repeat***

The image is only shown once. The background-attachment property specifies whether a background image should stay in one position or move as the user scrolls up and down the page. It can have one of two values:

1. fixed

The background image stays in the same position on the page.

2. scroll

The background image moves up and down as the user scrolls up and down the page.

## Background Position

When an image is not being repeated, you can use the background-position property to specify where in the browser window the background image should be placed.

This property usually has a pair of values. The first represents the horizontal position and the second represents the vertical.

If you only specify one value, the second value will default to
center.

You can also use a pair of pixels or percentages. These represent the distance from the top left corner of the browser window (or containing box). The top left corner is equal to 0% 0%. TheN  example shown, with values of 50% 50%, centers the image horizontally and vertically.

## CSS Gradients background-image

* CSS3 is going to introduce the
ability to specify a gradient for the background of a box. The gradient is created using the background-image property and, at the time of writing, different browsers required a different syntax.

Since it is not supported by all
browsers, it is possible to specify
a background image for the box
first (which would represent the
gradient) and then provide the
CSS alternatives for browsers
that support gradients.

On this page, we are focusing
on linear gradients. You can see
that in order to create a linear
gradient, we need to specify
two colors (that the gradient is
between).

## Contrast of background images

If you want to overlay text on a background image, the image must be low contrast in order for the text to be legible.

1. High Contrast

The majority of photographs have quite a high contrast, which means that they are not ideal for use as a background image.

2. Low Contrast

Image editing applications such as Photoshop and GIMP have tools that allow you to manually adjust your images to have lower contrast.

3. Screen

To overlay text on an image with high contrast, you can place a semi-transparent background color (or "screen") behind the text to improve legibility.

## SUMMARY

* You can specify the dimensions of images using CSS. This is very helpful when you use the same sized images on several pages of your site.

* Images can be aligned both horizontally and vertically using CSS.

* You can use a background image behind the box created by any element on a page.

* Background images can appear just once or be repeated across the background of the box.

* You can create image rollover effects by moving the background position of an image.

* To reduce the number of images your browser has to load, you can create image sprites.

# **Chapter (19)**

# PRACTICAL INFORMATION

## On-Page SEO

In every page of your website there are seven key places where keywords (the words people might search on to find your site) can appear in order to improve its findability.

1. Page Title

The page title appears at the top
of the browser window or on the tab of a browser. It is specified in the (title) element which lives
inside the (head) element.

2. URL / Web Address

The name of the file is part of the URL. Where possible, use keywords in the file name.

3. Headings

If the keywords are in a heading (hn) element then a search engine will know that this page is all about that subject and give it
greater weight than other text.

4. Text

Where possible, it helps to repeat the keywords in the main body of the text at least 2-3 times. Do not, however, over-use these terms, because the text must be easy for a human to read.

5. Link Text

Use keywords in the text that create links between pages (rather than using generic expressions such as "click here").

6. Image Alt Text

Search engines rely on you providing accurate descriptions
of images in the alt text. This
will also help your images show up in the results of image-based
searches.

7. Page Descriptions

The description also lives inside the (head) element and is specified using a (meta) tag. It should be a sentence that describes the content of the page. (These are not shown in the browser window but they may be displayed in the results pages of search engines.)

## How to Identify Keywords and Phrases

Determining which keywords to use on your site can be one of the
hardest tasks when you start to think about SEO. Here are six steps that will help you identify the right keywords and phrases for your site.

1. Brainstorm
2. Organize
3. Research
4. Compare
5. Refine
6. Map

## Analytics: Learning about your Visitors

As soon as people start coming to your site, you can start analyzing
how they found it, what they were looking at and at what point they are leaving. One of the best tools for doing this is a free service offered by Google called Google Analytics.

**Signing Up**

The Google Analytics service
relies on you signing up for an
account at:
www.google.com/analytics
The site will give you a piece of
tracking code which you need to
put on every page of your site.

**How it Works**

Every time someone loads a
page of your site, the tracking
code sends data to the Google
servers where it is stored.
Google then provides a webbased
interface that allows you
to see how visitors use your site.

**The Tracking Code**

A tracking code is provided
by Google Analytics for each
website you are tracking. It
should appear just before the
closing (head) tag. The code
does not alter the appearance of
your web pages.

## SUMMARY

* Search engine optimization helps visitors find your sites when using search engines.

* Analytics tools such as Google Analytics allow you to see how many people visit your site, how they find it, and what they do when they get there.

* To put your site on the web, you will need to obtain a domain name and web hosting.

* FTP programs allow you to transfer files from your local computer to your web server.

* Many companies provide platforms for blogging, email newsletters, e-commerce and other popular website tools (to save you writing them from scratch).

# **CHAPTER (9)**

# Flash, Video & Audio

## How Flash Works

Since the late 1990s, Flash has been a very popular tool for creating animations, and later for playing audio and video in websites.

Whether you are creating an animation or a media player in Flash, the files you put on your website are referred to as Flash
movies.

There are, however, several companies that offer Flash animations and slideshows, as well as video and audio players that you can use without purchasing this tool.

When you create a Flash file in
the Flash authoring environment,
it is saved with the .fla file
extension. In order to use this file on a web page it has to be saved in a different format known as SWF. (It has the .swf file
extension.)

When you export the movie
into SWF format, Flash creates
code that you can use to embed
the Flash movie in your page.
Traditionally, this code used the
HTML (object) and (embed) tags. However, now it is more common to use JavaScript

To view Flash, browsers need
to use a plugin (an extra piece of software that runs in the browser) called the Flash Player. Statistics commonly indicate
that 98% of browsers on
desktop computers have the
Flash plugin installed. (The
percentage of mobiles and
tablets with it is much less.)

There is not space in this book
to teach you how to create Flash
movies (there are many books devoted to that one topic), but
this chapter will show you how
to add Flash movies to your site.

## Use of Flash

Since 2005, a number of factors have meant that fewer websites are written in Flash or even use elements of Flash in their pages.

When Flash was first released,
it was developed to create
animations. The technology
quickly evolved, however, and
people started to use it to build
media players and even entire
websites.

Although Flash is still very
popular, in recent years people
have been more selective about
when they use it (and now rarely
consider building an entire
website in Flash).

## Timeline: Flash, VidEo & Audio

Web technologies change quickly. Here you
can see some of the changes in how animation,
video, and audio are created on the web.

# Video and Audio APIs

HTML5 comes with elements for embedding rich media in documents — (video) and (audio) — which in turn come with their own APIs for controlling playback, seeking, etc. This article shows you how to do common tasks such as creating custom playback controls.

## The HTMLMediaElement API

Part of the HTML5 spec, the HTMLMediaElement API provides features to allow you to control video and audio players programmatically — for example HTMLMediaElement.play(), HTMLMediaElement.pause(), etc. This interface is available to both (audio) and (video) elements, as the features you'll want to implement are nearly identical. Let's go through an example, adding features as we go.

## SUMMARY

* The HTMLMediaElement API makes a wealth of functionality available for creating simple video and audio players, and that's only the tip of the iceberg. See the "See also" section below for links to more complex and interesting functionality.

* Here are some suggestions for ways you could enhance the existing example we've built up:

1. The time display currently breaks if the video is an hour long or more (well, it won't display hours; just minutes and seconds). Can you figure out how to change the example to make it display hours?

2. Because (audio) elements have the same HTMLMediaElement functionality available to them, you could easily get this player to work for an (audio) element too. Try doing so.

3. Can you work out a way to turn the timer inner (div) element into a true seek bar/scrobbler — i.e., when you click somewhere on the bar, it jumps to that relative position in the video playback? As a hint, you can find out the X and Y values of the element's left/right and top/bottom sides via the getBoundingClientRect() method, and you can find the coordinates of a mouse click via the event object of the click event, called on the Document object.
 
# THE END
