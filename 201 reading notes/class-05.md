# Images

## Adding Images

*img*

To add an image into the page you need to use an (img) element. This is an empty element (which means there is no closing tag). It must carry the following two attributes:

src => This tells the browser where it can find the image file. This will usually be a relative URL pointing to an image on your own site. (Here you can see that the images are in a child folder called images.

alt => This provides a text description of the image which describes the image if you cannot see it.

title => You can also use the title attribute with the (img) element to provide additional information about the image. Most browsers will display the content of this attribute in a tootip when the user hovers over the image.

## Height & Width of Images

You will also often see an (img) element use two other attributes that specify its size:

*height*

This specifies the height of the image in pixels.

*width* 

* This specifies the width of the image in pixels.

* Images often take longer to load than the HTML code that makes up the rest of the page. It is, therefore, a good idea to specify the size of the image so that the browser can render the rest of the text on the page while leaving the right amount of space for the image that is still loading.

## Where to Place Images in Your Code

Where an image is placed in the code will affect how it is displayed. Here are three examples of image placement that produce different results:

1: before a paragraph The paragraph starts on a new line after the image.

2: inside the start of a paragraph The first row of text aligns with the bottom of the image.

3: in the middle of a paragraph The image is placed between the words of the paragraph that it appears in.

## Old Code: Aligning Images Horizontally

*align*

The align attribute was commonly used to indicate how the other parts of a page should flow around an image. It has 
been removed from HTML5 and new websites should use CSS to control the alignment of images

I have discussed it here because you are likely to come across it if you look at older code, and because some visual editors still insert this attribute when you indicate how an image should be aligned.

The align attribute can take these horizontal values:

*left*

This aligns the image to the left (allowing text to flow around its right-hand side).

*right*

This aligns the image to the right (allowing text to flow around its left-hand side).

## Old Code: Aligning Images Vertically

There are three values that the align attribute can take that control how the image should align vertically with the text that surrounds it:

* topUse the correct

This aligns the first line of the surrounding text with the top of the image.

* middle

This aligns the first line of the surrounding text with the middle of the image.

* bottom

This aligns the first line of the surrounding text with the bottom of the image.

## Three Rules for Creating Images

There are three rules to remember when you are creating images for your website which are summarized below. We go into greater detail on each topic over the next nine pages.

1. Save images in the right format

2. Save images at the right size

3. Use the correct resolution

## Cropping Images

When cropping images it is important not to lose valuable information. It is best to source images that are the correct shape if possible.

## HTML5: Figure and Figure Caption

*figure*

Images often come with captions. HTML5 has introduced a new (figure) element to contain images and their caption so that the two are associated. You can have more than one image inside the (figure)element as long as they all share the same caption.

*figcaption*

The (figcaption) element has been added to HTML5 in order to allow web page authors to add a caption to an image. Before these elements were created there was no way to associate an (img) element with its caption.

## Summary

* The (img) element is used to add images to a web page.

* You must always specify a src attribute to indicate the source of an image and an alt attribute to describe the content of an image.

* You should save images at the size you will be using them on the web page and in the appropriate format.

* Photographs are best saved as JPEGs; illustrations or logos that use flat colors are better saved as GIFs.

# Color

Every color on a computer screen is created by mixing amounts of red, green, and blue. To find the color you want, you can use a color picker.

* **RGB Values**

Values for red, green, and blue are expressed as numbers between 0 and 255. 

* **Hex Codes**

Values for red, green, and blue are expressed as numbers between 0 and 255. 


* **Color Names**

Colors are represented by predefined names. However they are very limited in number

* **Hue**

Hue is near to the colloquial idea of color Technically speaking however, a color can also have saturation and brightness as well as hue.

* **Saturation**

Saturation refers to the amount of gray in a color. At maximum saturation, there would be no gray in the color. At minimum saturation, the color would be mostly gray

* **Brightness**

Brightness (or "value") refers to how much black is in a color. At maximum brightness, there would be no black in the color. At minimum brightness, the color would be very dark.


## CSS3: Opacity, rgba

* CSS3 introduces the opacity property which allows you to specify the opacity of an element and any of its child elements. The value is a number between 0.0 and 1.0 (so a value of 0.5is 50% opacity and 0.15 is 15% opacity).

* The CSS3 rgba property allows you to specify a color, just like you would with an RGB value, but adds a fourth value to indicate opacity. This value is known as an alpha value and is a number between 0.0 and 1.0 (so a value of 0.5 is 50% opacity and 0.15 is 15% opacity). The rgba value will only affect the element on which it is applied (not child elements).


* Because some browsers will not recognize RGBA colors, you can offer a fallback so that they display a solid color. If there are two rules that apply to the same element, the latter of the two will take priority. To create the fallback, you can specify a color as a hex code, color name or RGB value, followed by the rule that specifies an RGBA value. If the browser understands RGBA colors it will use that rule. If it doesn't, it will use the RGB value.


## CSS3: HSL & HSLA

* HUE

* SATURATION

* LIGHTNESS

* ALPHA

## Summary

* Color not only brings your site to life, but also helps convey the mood and evokes reactions.

* There are three ways to specify colors in CSS: RGB values, hex codes, and color names.

* Color pickers can help you find the color you want.

* It is important to ensure that there is enough contrast between any text and the background color(otherwise people will not be able to read your content).

* CSS3 has introduced an extra value for RGB colors to indicate opacity. It is known as RGBA.

* CSS3 also allows you to specify colors as HSL values with an optional opacity value. It is known as HSLA.


# Text

## Typeface Terminology

* Serif 

Serif fonts have extra details on the ends of the main strokes of the letters. These details are known as serifs.

* Sans-Serif

Sans-serif fonts have straight ends to letters, and therefore have a much cleaner design.

* Monospace

Every letter in a monospace (or fixed-width) font is the same width. (Non-monospace fonts have different widths.)

## Specifying Typefaces font-family

* The font-family property allows you to specify the typeface that should be used for any text inside the element(s) to which a CSS rule applies.

* The value of this property is the name of the typeface you want to use. 

* The people who are visiting your site need the typeface you have specified installed on their computer in order for it to be displayed. 

* You can specify a list of fonts separated by commas so that, if the user does not have your first choice of typeface installed, the browser can try to use an alternative font from the list.

* It is also common to end with a generic font name for that type of font.

* If a font name is made up of more than one word, it should be put in double quotes.

* Designers suggest pages usually look better if they use no more than three typefaces on a page.

## Summary 

* There are properties to control the choice of font, size, weight, style, and spacing.

* There is a limited choice of fonts that you can assume most people will have installed.

* If you want to use a wider range of typefaces there are several options, but you need to have the right license to use them.

* You can control the space between lines of text, individual letters, and words. Text can also be aligned to the left, right, center, or justified. It can also be indented.

* You can use pseudo-classes to change the style of an element when a user hovers over or clicks on text, or when they have visited a link.

## JPEG vs PNG vs GIF

**TL;DR**

Use JPEG format for all images that contain a natural scene or photograph where variation in colour and intensity is smooth. Use PNG format for any image that needs transparency or for images with text & objects with sharp contrast edges like logos. Use GIF format for images that contain animations.

* **JPEG**

JPEG is a lossy compression specification that takes advantage of human perception. It can achieve compression ratios of 1:10 without any perceivable difference in quality. Beyond this, the compression artefacts become more prominent. Because JPEG compression works by averaging out colours of nearby pixels (read Discrete Cosine Transform), JPEG images are best suited for photographs and paintings of natural scenes where the variations in colour and intensity are smooth. However, if an image contains text or lines, where a sharp contrast between adjacent pixels is desired to highlight the proper shape, this lossy compression technique does not yield good results.

* **PNG**

PNG is a lossless image format using DEFLATE compression. No data is lost during compression and no compression artefacts are introduced in the image. For this reason, a PNG image would retain higher quality than an image than JPEG and would look a lot sharper, it would also occupy more space on the disk. This makes it unsuitable for storing or transferring high-resolution digital photographs but a great choice for images with text, logos and shapes with sharp edges.

* **GIF**

GIF is also a lossless image format that uses LZW compression algorithm. It was favoured over PNG for simple graphics in websites in its early days because the support of PNG was still growing. Given that PNG is now supported across all major devices and that PNG compression is about 5–25% better than GIF compression, GIF images are now mainly used only if the image contains animations.


## Colours

There is a significant difference in the number of colours that can be supported by these 3 formats.

**JPEG** images can support around 16 million colours. This is what makes them suitable for storing images of natural scenes.

**PNG** images mainly have two modes — PNG8 and PNG24. PNG8 can support upto 256 colours whereas PNG24 can handle upto 16 million colours like a JPEG image. Use PNG8 for simple shapes with fewer colours and PNG24 for high quality, complex logos and shapes with rounded corners on a transparent background.

**GIF** images are limited to 256 colours. If index transparency is used, then one of these 256 colours is assigned as transparent and the remaining 255 are used for other colours.


## Animation

Animation, in this case, refers to any change or movement in the image. It doesn’t necessarily have to have frame rates like an animated video, but essentially a part or the entire image changes with time.

Of these 3 formats, only GIF supports animation. This capability makes GIF format suitable for delivering engaging ads and banners. Of late, with the advent of companies Tumblr, 9Gag, Giphy etc. the use of GIF format for memes has picked up.

## THE END 