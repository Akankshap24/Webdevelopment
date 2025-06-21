# HTML 🖥️
 - It stands for Hyper Text Markup Language.
 - It is used mainly for ``Presentation`` purpose.
 - ``Markup`` refers to ``Marking up the content`` so that it can be presented exactly as required.
 - HTML to browser will display the presentation as need by the user.


## Evolution of HTML:

 - In Early 1960's GML and SGML are the languages used for ``Markup``.
 - Generic Markup Language and StandardGenericMarkUp Language were designed by CERN[Council for European Research and Nuclear] Labs.
 - In early 1990's ``Time Berner lee`` introduced ``WEB`` and a language for "WEB" that is ``HTML``[Open Source].
 - IETF(Internet Engineering Task Force) these people developed HTML for several years up to HTML3.1.
 - In 2004 ``WHATWG``(Web Hypertext Application Technology Work Group) took the responsibility of HTML and started the 
    version ``HTML4.0``.
 - Official website of WHATWG is "whatwg.org".
 - The latest version of HTML is ``HTML5``(2014).


### FAQs :-
#### Whats new in HTML5?
    HTML5  introduced new features to make webpages more browser and SEO friendly.
    SEO refers to "Search Engine Optimisation".
    Responsive Designs[users using webapplication using phones, so website should provide facility for user to use website]

## Browser Architecture 🌐💻🛠️

A ``browser`` is a software tool that allows users to access webpages on a client device. Popular browsers include:
- Chrome
- Firefox
- Edge
- Safari

Each browser consists of the following components:
### 1. User Interface (UI)
This includes elements such as the title bar, address bar, refresh button, etc., that allow users to interact with the browser.

### 2. Browser Engine
The browser engine is responsible for converting HTML and CSS into a format that the browser can understand. Different browsers use different browser engines, such as:

- **Gecko** (used by Firefox)
- **WebKit** (used by Safari)
- **Blink** (used by Chrome and Edge)
- **Chakra** (used by older versions of Edge)
- **SpiderMonkey** (JavaScript engine for Firefox)

### 3. Rendering Engine
This component is responsible for the presentation of processed content. It interprets the content from HTML and CSS into a visual display on the screen.

### 4. JavaScript Interpreter
Browsers use JavaScript for interactive functionality. The JavaScript interpreter converts JavaScript code into a format the browser can execute.

### 5. Networking
The networking component manages all network activities in the browser, including:

- Loading resources such as images, scripts, and stylesheets
- Handling the number of requests made per page
- Measuring the time taken to load content

### 6. UI Backend
This component contains the logic responsible for rendering the user interface, including buttons, checkboxes, and other input controls.

### 7. Data Persistence
Browsers store user data in different formats to enhance user experience, including:

- **Local Storage**: Stores data across sessions
- **Session Storage**: Stores data for the duration of a session
- **Cookies**: Store small amounts of data for stateful interactions with websites

## HTML Parsing in Browser

### Flow 
Markup 
   -> bytes 
      -> characters 
         -> Tokens [Tags] 
            -> Elements [Nodes] 
               -> DOM 
                  -> Layout 
                     -> Rendering 
                        -> Painting

*HTML       - presenting DOM* <br>
*JAVASCITPT - Modifying  DOM*

- HTML present content on browser using elements arranged in hierarchial order called "DOM".
- There are 100's of elements.

### HTML Elements are classified into 5 categories

### a. Normal Elements
- Elements which return a presentation directly on callback [without any additional attributes].
- Elements in HTML are built using tags.
- Normal elements require a start tag and end tag.
- Normal elements will start returning presentation but can’t stop implicitly.
- They require an explicit end tag.
- Usually require start and end tags.
	
- Example:
```HTML
<b>HELLO</b>
```
### b. Void Elements
- Void elements refer to elements that don’t return any presentation directly upon being rendered.
- The term "void" indicates that they have no return type.
- They can return specific content and stop implicitly.
- Void elements do not require an "end tag."

Example:
```html
<img src="image.jpg" alt="Image description">
```
### c. Raw Text Elements
- These elements are presented without a tag.<br>
		eg:: Temparature20C 45000/-<br>
		     Temparture&deg;C &#8377;45000/-
		     
Example:
```html
&copy; ©
&#8377;
&deg;
```

### d. RC Data Elements
- RC Data Elements, or Rich Text Content Elements, do not allow any other elements within their context.

Example:
```html
<textarea>
    Hello
    <b>pwian's</b>
</textarea 
```

### e. Foreign Elements
- Foreign elements are those that are not natively understood by every browser.
- You need to import a library that enables browser compatibility with these elements.

Example:
- SVG
- MathML
- Canvas


## HTML Page Structure

- Every HTML file must have static extensions called ".html or .htm"
- Every HTML page starts with documentation declaration from HTML5 version.<br>
 			<!doctype html><br>
	It is a indication to the browser engine that i am using latest features of HTML, if we don't specify the doctype then the
	browser engine understands the HTML has "HTML4" version.

- Every HTML page must have a documentation scope, It specifies the start and end of the document in browser.
#### eg: 
      <html> 
		document scope
		</html>

    eg#1.
	<!DOCTYPE html>
	<html>
        	document-1
	</html>
	<html>
        	document-2
	</html>
	     Note: If some changes needs to be done in document-1, then it creates a problem because browser does the below things
	<!DOCTYPE html>
	<html>
        	document-1 document-2
	</html>
   

#### Every document scope must have "lang" attribute.It is used to define language for the web page content.
	<html lang="en-IN">
	<html lang="en-US">
		eg:: amazon.com (USA) , amazon.in(IND)

#### Every document scope has 2 sections at high level.
	<!DOCTYPE html>
	<html>
        	<head>

        	</head>
        	<body>
                
        	</body>
	</html>
	
### HeadSection 
- It Comprises of the Content loaded into browser memory and later delivered to browser UI, so that we can reuse the content across multiple requests.
- It typically contains the following components
			a.link	 b.meta  c.style  d.scripts e.title

### title
-  It is used for browser and SEO.[Search Engine Optmisation]<br>
   Note: ROBOTS [Google BOT, WebCrawlers, WebSpiders]<br>
- Broswer uses title tag to display in "titlebar" and in "favourites".[While bookmarking the webpage]
- SEO uses title to display in search results.

### link  
- It is used to link any external document like css file or shortcut icon.
#### Note: favicon.ico -> size (16px to 32px), type(.ico)

					index.html
		<html lang="en-US">
			<head>
		 		<title>FashionStore</title>
		 		<link rel= 'shortcut icon' href='public/images/favicon.ico'/>
			</head>
		</html>


## Meta in head section
 - It is required for webpage to make it responsive and SEO Friendly.
 - The term meta refers to MetaData.
 - Meta data comprises of information about our webpage.
 - A responsive webpage can adjust according to device.
 - It can fit content to device screen[ipad,browser,phone,etc...]
 - To Test the responsivness pages, you can download and install
	     "chrome mobile simulator"

#### Add the following content in the head section:
```html
<meta name="viewport" content="width=device-width, initial-scale=1" />
```
- **a. viewport**: It refers to the screen size and its dimensions.
- **b. width**: It refers to the current page content width.
- **c. initial-scale**: It refers to the zoom level (1 = 100%).

#### eg#1.
``` html
 <!DOCTYPE html>
<html>
    <head >
        <meta name="viewport" content="width=device-width, initial-scale=200">
	<title>
		Fashion Store
	</title>

    </head>        
        <body>
            Many of our Services allow. 
    </head>
</html>
```


2. ``` html
       <meta http-equiv="refresh" content="5">
   ```
	http-equiv : refers to request handler, which can process your request for page by refreshing every few seconds<br>
	content    : it defines the no of seconds

- Meta provides following attributes to make our page SEO Friendly
	```html
	<meta name = "keywords"  content = "some keywords used for finding our site"/>
	<meta name="description" content = "something abour our result"/>
	<meta charset="UTF-8">
	```
	a. UTF-8 :: Unicode Translation Format(applicable for english alphabets)<br>
	b. UTF-16, UTF-32......

#### eg#1.					index.html
```html
<html lang="en-IN">
    <head >
        <meta name="viewport" content="width=device-width, initial-scale=200">
        <meta http-equv="refresh" content="5">
        <meta name ="keywords" content="kids,Mens,Womens fashion best offers">
        <meta name = "description" content="online fashion store with best offers ">
    </head>
</html>
```

4. style : It is used to embed css into webpage
    ```html
		<style type ='text/css'>
		</style>
    ```
5.  ```html
    <script type = 'text/javascript'>
    </script>
	```

## HTML BODY SECTION 
- It comprises of the content which is rendred directly in browser.
- It is defined with ``<body>`` token and it contains some important attributes.
### Attributes
**bgcolor** :It sets background color for the page.<br>
**text**    : It sets text color 

=>HTML colors are defined by using 3 techniques <br>
a.**Color name**			
#### eg:
```html
	<body bgcolor="red" text="white">
	<p>.....</p>
	</body>
```
 
b. **Color shade name**
   - HTML also supports hundreds of color shade names
     - Darkcyan
     - Lightcyan
     - Lightgreen

c. **Hexadecimal Code**
   - Hexadecimal colors are basically “RGB” colors:
     - R-Red, G-Green, B-Blue
     - Hexadecimal number system is a 16-base system, using 16 different values ranging from “0 to F.”
     - Hexadecimal colors can be defined in 3 or 6 characters, followed by a hash “#”:
       - **3 Chars Code:**
         - `#RGB`
       - **6 Chars Code:**
         - `#RRGGBB`
     - Red, Green, and Blue values range from “0 to F”:
       - Hexadecimal values: 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, a, b, c, d, e, f
         - [0 is minimum, f is maximum]
         - First place is for **Red**
         - Second place is for **Green**
         - Third place is for **Blue**

#### Example: Hexadecimal Color Codes

| Hex Code  | Color  | Short Code |
|-----------|--------|------------|
| #FF0000   | Red    | #F00       |
| #00FF00   | Green  | #0F0       |
| #0000FF   | Blue   | #00F       |
| #FFFF00   | Yellow | #FF0       |
| #000000   | Black  | #000       |
| #FFFFFF   | White  | #FFF       |

### 3. Background

It sets a background image to the body section.

**Syntax:**
```html
<body background="" />
```
> [!NOTE]
> we can control images only through css attributes.
  These attributes are defined in ``style`` manner.

CSS attributes for background are:

| Attribute               | Values                                     |
|-------------------------|--------------------------------------------|
| background-repeat      | repeat \| no-repeat \| repeat-x \| repeat-y |
| background-size        | contain \| cover \| auto \| width & height in pixels |
| background-position    | top \| center \| right \| left    |
| background-attachment  | fixed \| scroll                       |
    
- **contain**: Resize the background image to ensure it is fully visible, scaling it to fit inside the container without cropping.
- **cover**: Resize the background image to cover the entire container, even if part of the image is cropped to maintain aspect ratio.

Example:

```html
<style>
     body {
         background-repeat: no-repeat;
         background-size: 100%;
         background-position: center center;
         background-attachment: fixed;  
     }
</style>

<body background="public/images/background-banner.jpg">
    ........
    ........
    ........
</body>
```
### 4. align
It is used to align the body content to the left, right, center, or justify.

   **Syntax**: 
   ```html
   <body align="left|right|center|justify">
   </body>
   ```
   
- **left**: It sets the text left-aligned.<br>
- **right**: It sets the text right-aligned.<br>
- **center**: It sets the text center-aligned.<br>
- **justify**: It stretches the text of a paragraph to set the width of all lines equal.

### 5. margin
 Sets space between the content and the page edges.
- **left margin**: Sets the space between the content and the left edge of the page.
- **right margin**: Sets the space between the content and the right edge of the page.
- **bottom margin**: Sets the space between the content and the bottom edge of the page.
- **top margin**: Sets the space between the content and the top edge of the page.

   **Example**:
   ```html
   <body align="justify" topmargin="25" leftmargin="50" bottommargin="50" rightmargin="50">
   </body>
   ```
  ### 6. 
  **Vlink** : It sets colour for visited links in a page  
  **alink** : It sets colour for active  links in  a page  
  ```html
  <body vlink="grey" alink="red">
            <a href="http://www.flipkart.com">FLIPKART</a> 
            <a href="http://www.amazon.in">AMAZON</a>   
            <a href="http://www.myntra.com">MYNTRA</a>  
   </body>  
   ```
## Semantics in Body Section  
- An element used for a specific purpose.  
- HTML has more than 100 of semantics according to MDN.  
- WHATWG(HTML), W3C(WEB), Javascript(ECMA) for these 3 people documentation is prepared by MDN (Mozilla Development Network).  
- HTML5 introduced semantics for body section to make it more SEO [Search Engine Optimization] friendly.  
- Old websites are not SEO friendly, but by using HTML5 we make webpages SEO friendly.

## Body section semantics for Layout Design  
- HTML4 uses table element for designing a "Layout".  
- Table is not SEO Friendly  
- Table leads to a situation known as "Kiss-Of-Death". [refer image for this problem]  
- HTML5 introduced new "Semantics" for designing a Layout.  
- The new semantics will make a page SEO Friendly.  
- The new layout semantics are  
    `<aside>` `<article>`  `<header>`  `<footer>` `<div>` `<span>` `<figure>` `<figcaption>`  `<dialog>`  `<main>`  `<section>`  `<div>`  `<span>`  

 **div and span tag**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>layout</title>
    <style>
        div {
            border: 2px solid black;
            margin: 5px;
            padding: 5px;
        }
        span {
            background-color: rgb(0, 174, 255);
        }
    </style>
</head>

<body>
    <div>
        Web Development
        <div>
            FrontEnd
            <div>
                HTML
                It is a <span>markup</span> language
            </div>
            <div>
                CSS
                It is a styling language
            </div>
        </div>

        <div>
            BackEnd
            <div>
                MongoDB
                It is a database
            </div>
            <div>
               Node.js
               It is a server-side scripting language
            </div>
        </div>
    </div> 
</body>
</html>
```

>[!NOTE] 
The `<span>` tag is much like the `<div>` element,but `<div>` is a block-level element and `<span>` is an inline element.

- **Padding** is used to create space around an element's content, inside of any defined borders.  
   CSS has properties for specifying the padding for each side of an element:
   
   1. padding-top
   2. padding-right
   3. padding-bottom
   4. padding-left

>[!Note] 
padding : top left right bottom

#### eg#1
    padding: 25px;

***all four paddings are 25px***

2. `<header>`
   1. It is used to configure the header section of a webpage.  
   2. Typically, every header of a webpage comprises:
      - a. BrandName  
      - b. BrandIcon  
      - c. NavBar  
      - d. Shortcut Buttons, etc.

```html
<header>
	content of the header
</header>
```
It is a container that is used to display a top margin on the page.
Typically header is a webpage comprises of brand- name,logo,shortcut buttons,navigation etc...

## CSS style attributes  
To work with any of the fonts we use these attributes in CSS:

**font-size**: It changes the character size. [unit: px]  
**font-weight**: It changes in bold.  
**font-style**: It changes in italics.  
**font-family**: It sets text style by using font-family. [Arial, Times New Roman,....]

- **margin**: 
   - margin-left: 
   - margin-right: 
   - margin-top: 
   - margin-bottom: 

- **display**: It can display the elements in the container with various styles:
   -  none
   -  block : just like `<p>`
   -  inline : just like `<span>`
   -  inline-block
   -  grid : Displays an element as a block-level grid container
   -  flex : Displays an element as a block-level flex container

- **justify-content**: It can justify the contents in the container with the following values:
   - `space-between`: Items will have space between them
   - `space-around`: Items will have space before, between, and after them
   - `space-evenly`: Items will have equal space around them

- **padding**: It sets space around contents in all directions 
   - padding-bottom
   - padding-top
   - padding-right
   - padding-left

- **border** - It sets border style, side, and color for the container.  
- **border-radius** - It sets rounded container.  
- **text-align**- It aligns text left, center, right, or justify. 

> [!NOTE] 
We can't change height and width of any `<span>` element using CSS.  
To set width and height of a `<span>` we need to go for `display: inline-block`.

`<nav>` It is used to configure the navigation area in a webpage. It comprises of nav items or shortcut buttons.

`<article>` It is a container element that keeps the highlights of webpage content. It is typically the offers, announcement, news, updates, etc.

`<footer>`  It defines the content to display at the bottom margin of a web page.Typically, the footer comprises copyrights, contact details, social bars, services, etc.

`<aside>`   It defines the content which is not relative to the current context or navigates the user to another website.It contains the content outside the current context.
  
**Syntax**:
```html
<aside>
    social media ads,....
</aside>
```
> [!Note]
> - `display: flex` -> Keeps flexible columns, which change according to the width of the screen.  
> - `display: grid` -> Keeps a fixed number of columns.  
> - Default screen width is 1200px, so the maximum number of columns on a page is 12.  
> - We can split the grid into columns using `grid-template-columns`.  
> - Each column's size can be set using pixels or fractions.  
>   - **Example**: `200px 5fr`  
> - Pixels are fixed, and fractions are responsive (will adjust according to the width of the screen).

**Syntax**:
```css
footer {
    display: grid;
    grid-template-columns: 240px;
}
```
> [!Note]
 Selecting child and sibling in CSS  
`parent child { ... }`  -> Child selector  
`ElementA + ElementB { ... }`  -> Adjacent sibling  
`ElementA ~ ElementB { ... }`  -> All elements after a specific element  

### Designing a section area and main area  
**Section**: It defines the content between the header and footer area. Typically, all website content is kept in the section.<br>
  **Syntax**:
  ```html
  <section>
      // content
  </section>
   ```
**main**: It is considered the entry point; the user can start using the website through an entry point called main.<br>
  **Syntax**:
  ```html
  <main>
      // entry point
  </main>
  ```
### Displaying the content in the center  
1. Keep all the contents in one container.
   ```html
   <body>
       <div>
           // your content here
       </div>
   </body>
   ```
2. `body` is the container here which would display the contents in the center with the following attributes:

   ```css
   body {
       display: flex;
       justify-content: center;
       align-items: center;
       height: 100vh;
   }
> [!Note] 
> - justify-content: center (horizontal)  
> - align-items: center (vertical)  

### dialog  
- It is a popup created for the page.
- Syntax:
  ```html
  <dialog open="">
      // content
  </dialog>
  ```
- You can keep any content in a dialog, but it is hidden by default.
- You can show/hide the dialog using the `open` attribute.
- You can control the dialog dynamically using JavaScript.

HTML basic entities and semantics for body  

a. **Line break `<br>`**  
   - Browsers ignore the line breaks given in the editor.
   - You have to manually add a line break by using the `<br>` element.

   **FAQ: What is the difference between `<br>` and `<br/>`?**
   - There is no such element called `<br/>` in HTML.
   - Always use only `<br>`.
   - `<br/>` is used to indicate that it is a self-ending or void element (in XHTML).

b. **Blank Spaces**  
   - Browser ignores additional spaces between words and characters.
   - Browser allows only one character space between words or characters.
   - To add a manual space, you have to use `&nbsp;` (non-breaking space).
   - It is a "Raw Text Element".

c. **Pre-formatted Text**  
   - It is used to present the content exactly as defined in the source code.  
   - It will preserve the spaces and line breaks as defined in the editor.  
   - The content must be defined within the `<pre>` element.  

d. **Code Element**  
   - `<code>` is an element used to define a code snippet in a web page.  
   - It helps the browser and SEO understand that the enclosed content is some computer code.  

e. **Variables in HTML Code Presentation**  
   - You can use the `<var>` element for variables in HTML.  
   - Variables are designated using `<var>` in code snippets.  

f. **Sample Template for a Code**  
   - Use the `<samp>` element to present sample output.  
   - It is used for comments and captions on a page.  

### General Syntax  
```html
<samp>caption about the program</samp>
<code>
    <pre>
        <!-- Code about the caption -->
    </pre>
</code>
```

### Small Text and Large Text  
- `<small>content</small>`: It sets the letter size to small.  
- `<big>large</big>`: It sets the letter size to large.  

>[!Note]
In CSS we adjust the font we use "font-style", In HTML we have <font> but its not suggestible.<br>

**Example**:  
```html
<body>
    Normal Text<br>
    <small>Small Text</small><br>
    <big>Large Text</big>
</body>
```
### Details and Summary
- It is used to display the content in detail only when required.  
- It allows you to expand and collapse your content.  
- It saves screen space. 

**Syntax**:
```html
<details>
    <summary> Your Title </summary>
    some text…
</details>
```
- You can specify “open” attribute to show the details.

### Data List with Terms and Definitions:  
- A Data List is defined with `<dl>`.  
- A Data List is a collection of terms defined with `<dt>` and definitions defined with `<dd>`.  

**Syntax**:  
```html
<dl>
    <dt>Term</dt>
    <dd>Definition</dd>
    <dt>Term</dt>
    <dd>Definition</dd>
    <dd>Definition</dd>
</dl>
```

>[!Note] 
>1. `<dt>` and `<dd>` have some default alignment, making them easy for presentation.  
>2. `<dl>` has the capability to display in columns using a grid (`<dt>` -> one column and `<dd>` -> another column).  

>[!Note] 
>We can make content sticky on a webpage using the CSS property:  
```css
dt {
    position: sticky;
    top: 0;
}
```

### Field Set and Legends  
- A `<fieldset>` is a container with a frame.  
- A `<legend>` puts a caption for the field set.  

**Syntax**:  
```html
<fieldset>
    <legend>Title</legend>
    Your content…
</fieldset>
```
In CSS, we can set a shadow for any container using the `box-shadow` property. 

The `box-shadow` property takes four values:

```css
box-shadow: horizontal vertical blur color;
```
The unit of horizontal vertical blur is `pixels`.

### Headings in HTML

- Headings need a different appearance in page.  
- HTML provides pre-defined heading levels.  
- HTML headings levels are defined by using `<hn>`.  
- “n” refers to level number from 1 to 6.  
- They are not mainly meant for 'appearance' but also for 'SEO friendly'.  

### FAQ: 
#### 1 Why to use heading element for headings?

- Heading elements will make your topics SEO friendly.  
- SEO can identify the topics on your page if they are defined in heading.

>[!Note]
>- The effect of headings can be give without
>- `<hn>` tags also, then why we need <hn> tags
>- `<hn>` tags are given to make page SEO friendly which is as shown below


#### 2. Can we change the appearence of `<hn>` tags?
**Ans.** yes possible using css styling attributes.

#### 3. Can we remove the default style defined for Heading?

**Ans.** Default styles for headings include:

- `font-weight: bold`
- `font-size` (varies by level)
- `display: block`

To remove or control these default styles, we use **CSS inheritance values**.  
You can use the `unset` value in CSS to remove the browser's default styles.

```css
h1, h2, h3, h4, h5, h6 {
  all: unset;
}
```

>[!NOTE]
> - Don’t use headings to highlight any word or sentence within a paragraph.  
> - Headings, by default, have a line break above and below.  
> - Avoid using too many headings on a single page — excessive use may negatively affect SEO and can mark your page as spam.

### FAQ

#### Q: Why use heading elements for headings?
**Ans:** Heading elements (`<h1>` to `<h6>`) provide semantic meaning to the content, improve accessibility, and help with SEO by clearly defining the document structure.

---

#### Q: Why do we have to use heading elements for giving headings? Can't we just configure using HTML text styles and CSS?
**Ans:** While you *can* visually style text with HTML and CSS, using heading elements ensures semantic structure, which is important for screen readers, search engines, and document hierarchy.

---

#### Q: Can we change the appearance of `<hn>` tags?
**Ans:** Yes, the appearance of any heading tag (`<h1>` to `<h6>`) can be fully customized using CSS (e.g., changing font-size, color, margin, etc.).

---

#### Q: Can we remove the default style defined for Heading?
**Ans:** Default styles for headings include:
- `font-weight: bold`
- `font-size`
- `display: block`

To remove these defaults, we use CSS inheritance values like `unset`:

```css
h1, h2, h3, h4, h5, h6 {
  all: unset;
}
```
## Paragraphs and Blockquotes

- HTML ignores line breaks and paragraph marks by default.
- You must manually define paragraphs using the `<p>` element.
- The `<p>` element supports the `align` attribute to set text alignment: `left`, `center`, `right`, or `justify`.
- Paragraphs automatically include line breaks before and after.

**Syntax:**

```html
<p>Your Content</p>
<p align='left/right/center/justify'>Your Content</p>
```
## Working with `<blockquote>` Tag

- `<blockquote>` is similar to a paragraph but includes **left and right indentation** for the text.  
  *(Indentation refers to the space between the margin and the text.)*
- It is defined using the `<blockquote>` element.
- In SEO, `<blockquote>` is treated as a **summary or highlighted content** on a page.
- It is mainly used for **summary representation** or quoting external sources.

## Working with `<blockquote>` Tag

- `<blockquote>` is similar to a paragraph but includes **left and right indentation** for the text.  
  *(Indentation refers to the space between the margin and the text.)*
- It is defined using the `<blockquote>` element.
- In SEO, `<blockquote>` is treated as a **summary or highlighted content** on a page.
- It is mainly used for **summary representation** or quoting external sources.

**Example Syntax:**

```html
<blockquote>
  This is an example of blockquoted text with indentation.
</blockquote>
```

#### FAQ: How to set the first-line indent for a paragraph or blockquote?

**Ans.**  
You can set the first-line indent using the `text-indent` CSS property.

**Example:**

```css
blockquote {
  text-indent: 100px;
}
```

#### 2. How to set line space, word space, and character space in a paragraph?

**Ans.**  
You can control spacing in a paragraph using the following CSS properties:

- `line-height` → sets the **line spacing**
- `word-spacing` → sets the **space between words**
- `letter-spacing` → sets the **space between characters**

**Syntax:**

```css
p {
  line-height: 10px;
  word-spacing: 5px;
  letter-spacing: 15px;
}
```

#### 3. How to set a DropCap?

**Ans.**  
To create a **DropCap** (large first letter in a paragraph), follow these steps:

- Use the `::first-letter` pseudo-element to target the first letter.
- Apply desired font properties like `font-size`, `font-weight`, and `font-family`.
- Use `float: left` to align it beside the paragraph text.

**Syntax:**

```css
p::first-letter {
  font-size: 50px;
  font-weight: bold;
  float: left;
  font-family: "Brush Script MT", cursive;
  color: blue;
  padding-right: 2px;
}
```

### 4. How to display a paragraph as a continuous paragraph?

**Ans.**  
While using CSS Grid is possible, it's not ideal for this use case.  
Instead, we can use the **CSS `columns` attribute** to display a paragraph in a continuous, multi-column format.

**Example Syntax:**

```css
section {
  columns: 5;
  column-gap: 20px;
  margin-top: 25px;
  column-rule: 2px dotted black;
}
```

## Text Formatting in HTML

- You can change text formatting using the `<font>` tag.
- With `<font>`, you can modify:
  - `face` → font family  
  - `size` → 1 to 7 levels (increasing order)  
  - `color` → named colors or hex codes

**Syntax:**

```html
<font face="Arial" size="4" color="blue">Your Text</font>
```

