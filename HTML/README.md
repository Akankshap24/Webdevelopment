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
