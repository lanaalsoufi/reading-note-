# ***HTML & CSS***
## **Chapter(1)**
### ***Structure***

**HTML Describes the Structure of Pages** 

The HTML code is made up of characters that live inside angled
brackets — these are called HTML elements. Elements are usually
made up of two tags: an opening tag and a closing tag. (The closing tag
has an extra forward slash in it.) Each HTML element tells the browser
something about the information that sits between its opening and
closing tags .

* body : 

Everything inside this element is
shown inside the main browser
window.

* head :


This contains information
about the page (rather than
information that is shown within
the main part of the browser
window that is highlighted in
blue on the opposite page).
You will usually find a title
element inside the head
element

* Title :

The contents of this
element are either shown in the
top of the browser, above where
you usually type in the URL of
the page you want to visit, or
on the tab for that page (if your
browser uses tabs to allow you
to view multiple pages at the
same time). 

**Creating a Web Page on a PC**

1. Start All Programs (or Programs) Accessories Notepad, You might also like to download a free editor called Notepad++ from notepad-plus-plus.org.

2. Type the code shown on the right

3. Go to the File menu and select Save as... You will need to save the file somewhere you can remember. If you like, you could create a folder for any examples that you try out from this book. Save this file as first-test.
html. Make sure that the Save as type drop down has All Files selected.

4. Start your web browser. Go to the File menu and select Open. Browse to the file that you just created, select it and click on the Open button. The result should look something like the screen shot to the left.



- HTML Pages ages are text documents.

- HTML uses tags (characters that sit inside angled
brackets) to give the information they surround special
meaning.

- Tags are often referred to as elements.

- Tags usually come in pairs. The opening tag denotes
the start of a piece of content; the closing tag denotes
the end.

- Opening tags can carry attributes, which tell us more
about the content of that element.

- Attributes require a name and a value.

- To learn HTML you need to know what tags are
available for you to use, what they do, and where they
can go.


## **Chapter(2)**

### ***Extra Markup***

**There are some characters that are used in and reserved by HTML code. (For example, the
left and right angled brackets.)** 

1. Therefore, if you want these characters to appear on your page you need to use what are termed "escape" characters (also known as escape codes or entity references). For example, to write a left angled bracket, you can use either &lt; or &#60;. For an ampersand, you can use either &amp; or &#38;.

2. There are also special codes that can be used to show symbols such as copyright and trademark, currency symbols, mathematical characters, and some punctuation marks. For example, if you want to include a copyright symbol on a web page you can use either &copy; or &#169;

3.  When using escape characters, it is important to check the page in your browser to ensure that the correct symbol shows up. This is because some fonts do not support all of these characters and you might therefore need to specify a different font for these characters in your CSS code.

* DOCTYPES tell browsers which version of HTML you
are using.

* You can add comments to your code between the <!-- and --> markers.

* The id and class attributes allow you to identify particular elements.

* The <div> and <span> elements allow you to group block-level and inline elements together.

* <iframes> cut windows into your web pages through which other pages can be displayed.

*  The <meta> tag allows you to supply all kinds of information about your web page.

*  Escape characters are used to include special characters in your pages such as <, >, and ©.


## **Chapter(17)**
### ***HTML5 Layout***

**Headers & Footers**

The header and footer elements can be used for:

* The main header or footer that appears at the top or bottom of every page on the site.

* A header or footer for an individual article or section within the page.

**Navigation**

* The nav element is used to contain the major navigational blocks on the site such as the primary site navigation.

* Going back to our blog example, if you wanted to finish an article with links to related blog posts, these would not be counted as major navigational blocks and therefore should not sit inside a nav element.

* At the time of writing, some of the developers that were already using HTML5 decided to use the nav element for the links that appear at the bottom of every page (links to things like privacy policy, terms and conditions and accessibility information). Whether this will be widely adopted is still yet to be seen

**Articles**

* The article element acts as a container for any section of a page that could stand alone and potentially be syndicated.

* This could be an individual article or blog entry, a comment or forum post, or any other independent piece of content.


* If a page contains several articles (or even summaries of several articles), then each individual article would live inside its own article element.


* The article elements can even be nested inside each other. For example, a blog post might live inside one article element and each comment on the article could live inside its own child article element.



1. The new HTML5 elements indicate the purpose of different parts of a web page and help to describe its structure.


2. The new elements provide clearer code (compared with using multiple div elements).


3. Older browsers that do not understand HTML5 elements need to be told which elements are block-level elements.

4. To make HTML5 elements work in Internet Explorer 8 (and older versions of IE), extra JavaScript is needed, which is available free from Google.


## **Chapter(18)**
### ***Process & Design***

***WireFrames***


A wireframe is a simple sketch of the key information that needs to go on each page of a site. It shows the hierarchy of the information and how much space it might require.


* lot of designers will take the elements that need to appear on each page and start by creating wireframes. This involves sketching or shading areas where each element of the page will go (such as the logo, primary navigation, headings and main bodies of text, user logins etc).

* By creating a wireframe you can ensure that all of the information that needs to be on a page is included.


* You should not include the color scheme, font choices, backgrounds or images for the website in the wireframe. It should focus on what information needs to be on each page and create a visual hierarchy to indicate the most important parts of each page


* The wireframes make design easier because you know what information needs to appear on which page before considering


* how the the page should look. It can be very helpful to show the wireframes of a site to a client before showing them a design. It enables the client to ensure the site has all the functions and information it needs to offer.


* If you just present a site design to a client, it is common for them to focus on how the site looks, which means they may not raise issues about its function after the site has been built.


# THE END
