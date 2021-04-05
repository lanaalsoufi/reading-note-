<img src ="https://media.geeksforgeeks.org/wp-content/cdn-uploads/20191219190325/CSS5.png">


# **Introducing CSS**

CSS allows you to create rules that specify how the content of an element should appear. For example, you can specify that the background of the page is cream all paragraphs should appear in gray using the Arial typeface, or that all level one headings should be in a blue, italic, Times typeface.

## **Example Styles:**

 **Boxes :**

* Width and height 

* Borders (color, width, and style)

* Background color and images 

* Position in the browser window.

**Text :**

* Typeface

* Size

* Color

* Italics, bold, uppercase, lowercase, small-caps

**Specific :**

There are also specific ways in which you can style certain elements such as lists, tables, and forms.


## **CSS Associates Style rules with HTML elements**

CSS works by associating rules with HTML elements These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: a selector and a declaration.

* This rule indicates that all (p) elements should be shown in the Arial typeface. 

* **Selectors** indicate which element the rule applies to. The same rule can apply to more than one element if you separate the element names with commas.

* **Declarations** indicate how the elements referred to in the selector should be styled. Declarations are split into two parts (a property and a value), and are separated by a colon


## **CSS Properties Affect How Elements Are Displayed**

CSS declarations sit inside curly brackets and each is made up of two parts: a property and a value, separated by a colon. You can specify several properties in one declaration, each separated by a semi-colon.

* This rule indicates that all (h1), (h2) and (h3) elements should be shown in the Arial typeface, in a yellow color

* **Properties** indicate the aspects of the element you want to change. For example, color, font, width, height and border.

* **Values** specify the settings you want to use for the chosen properties. For example, if you want to specify a color property then the value is the color you want the text in these elements to be.


## **Using External CSS**

* ***link***

The (link) element can be used in an HTML document to tell the browser where to find the CSS file used to style the page. It is an empty element (meaning it does not need a closing tag), and it lives inside the (head) element. It should use three attributes:

1. href

This specifies the path to the CSS file (which is often placed in a folder called css or styles).

2. type

This attribute specifies the type of document being linked to. The value should be text/css.

3. rel

This specifies the relationship between the HTML page and the file it is linked to. The value should be stylesheet when linking to a CSS file.


## **CSS Selectors**

1. Universal Selector

2. Type Selector

3. Class Selector

4. ID Selector

5. Child Selector

6. Descendant Selector

7. Adjacent Sibling Selector

8. General Sibling Selector


## **Summary**

* CSS treats each HTML element as if it appears inside its own box and uses rules to indicate how that element should look.

* Rules are made up of selectors (that specify the elements the rule applies to) and declarations (that indicate what these elements should look like).

* Different types of selectors allow you to target your 
rules at different elements.

* Declarations are made up of two parts: the properties of the element that you want to change, and the values of those properties. For example, the font-family property sets the choice of font, and the value arial specifies Arial as the preferred typeface.

* CSS rules usually appear in a separate document although they may appear within an HTML page.



<img src ="https://cdn.educba.com/academy/wp-content/uploads/2020/02/CSS-Color-Generator.jpg">


# **Color**

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


## **CSS3: Opacity, rgba**

* CSS3 introduces the opacity property which allows you to specify the opacity of an element and any of its child elements. The value is a number between 0.0 and 1.0 (so a value of 0.5is 50% opacity and 0.15 is 15% opacity).

* The CSS3 rgba property allows you to specify a color, just like you would with an RGB value, but adds a fourth value to indicate opacity. This value is known as an alpha value and is a number between 0.0 and 1.0 (so a value of 0.5 is 50% opacity and 0.15 is 15% opacity). The rgba value will only affect the element on which it is applied (not child elements).


* Because some browsers will not recognize RGBA colors, you can offer a fallback so that they display a solid color. If there are two rules that apply to the same element, the latter of the two will take priority. To create the fallback, you can specify a color as a hex code, color name or RGB value, followed by the rule that specifies an RGBA value. If the browser understands RGBA colors it will use that rule. If it doesn't, it will use the RGB value.


## **CSS3: HSL & HSLA**

* HUE

* SATURATION

* LIGHTNESS

* ALPHA

## **Summury**

* Color not only brings your site to life, but also helps convey the mood and evokes reactions.

* There are three ways to specify colors in CSS: RGB values, hex codes, and color names.

* Color pickers can help you find the color you want.

* It is important to ensure that there is enough contrast between any text and the background color(otherwise people will not be able to read your content).

* CSS3 has introduced an extra value for RGB colors to indicate opacity. It is known as RGBA.

* CSS3 also allows you to specify colors as HSL values with an optional opacity value. It is known as HSLA.