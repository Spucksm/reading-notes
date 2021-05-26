# Structure Web Pages with HTML
## Table of Contents
  1. [Home](README.md)
  2. [Markdown](markdown.md)
  3. [Text-Editor](text-editor.md)
  4. [Day 2 Morning lecture notes](lecture_notes.md)
  5. [Reading 02 Day 1](reading02.md)
  6. [Reading 03 Day 2](reading03.md)
## Contents
* the Definitive guide: How To Create Your First Wireframe
* Mozilla HTML Basics
* Semantics
### The Definitive Guide: How to create Your First Wireframe
#### Introduction to wireframing
    * What is a wireframe
        *practice which allows dev to define and plan the info hierarchy of the website design (step 1)
    * examples of wireframes
        * Can be made in paint or use shapes on a white board, easist way is hand sketched on a plan old napkin. Start hand drawn then transfer to electronic later on if needed for beginers.
    * Things to consider when choosing a wireframing process
        * Wireframe> Interactive Prototype > Visual> Design
        * Sketch> Code
        * Sketch> Wireframe> Hi-Def Wireframe> Visual> Code
        * Sketch> Wireframe> Visual> Code
    * The best tools for wireframing
        * UXPin
        * InVision
        * Wireframe.cc
#### how to make your wireframe in six steps
    * Do your research
        1. who is the audience for the website
        2. complementing with competitor and industry research
    * Prepare your research for reference
        * Make a cheat sheet of the date from the research
    * Make sure you have your user flow mapped out
        * Things can get messy quickly. Keep your goals handy and your widows organized.
    * Draft, don't draw. Sketch, don't illustrate
        * This is a rough picture to drive your coding. This is not a Mona Lisa.
    * Add some detail and get testing
    * Start turning your wireframes into prototypes
#### How to make your wireframe good: Three key principles
    * Maintain clarity
    * Gain user confidence
    * Simplicity is key

### Mozilla HTML Basics
    #### So What is HTML?
        * HTML- Hypertext Markup Language
        * A markup language that defines the structure of the contect.
    The main parts
        1. the opening tag: consists of the name of the element, wrapped in opening and closing angle brackets.
        2. The closing tag: includes a foreward slash before element name. Says where the element ends.
        3. The content: is just text
        4. The element: putting all three together
    Attribute
    * contain extra informaion within the element
    Nesting elements
    * puting elements within other elements
    example ```<strong></strong>``` emphasized the word very.
    (p)My cat is <strong>very</strong> grumpy.</p>
    #### Anatomy of an HTML document
    * <!DOCTYPE html> - doctype. a required preamble for modern html
    * <html></html>- this element wraps all the content on the entire page. everything on the page will fall between the opening and closing tag
    * <head></head>- acts as a container for all the stuff you want to include on the HTML page taht isn't the contect the viewer sees.
    <meta charset="utf-8>- sets the character set the document should use to UTF-8.
    * <title></title>- sets the title of the page
    * <body></body>- contains all the content of the page the end user will see
    * Images
        *<img src="images/firefox-icon.png" alt="my test image">
    * Headings
        * <h1>My main title</h1>
        * <h2>My top level heading</h2>
        * <h3>My subheading</h3>
        * <h4>My sub-subheading</h4>
    * paragraphs
        * <p></p>
    * Lists
        * Unordered
            * <ul>
                * <li></li>
                * <li></li>
                </ul>
        * Ordered
            * <ol>
                * <li></li>
                * <li></li>
            *</ol>
    * links
        * <a href="https://www.mozilla.org/en-us/about/manifesto/">Mozilla Manifesto</a>
### Semantics
    * refers to the meaning of a piece of code- what effect does running that line of javascript have? or what purpose or role does that html element have? not what does it look like.
    Semantics in JavaScript
        *consider a function that takes a string parameter, and returns an <li> element with that string as its textcontent. Would I need to look as the code to understand what the function did if it was call build('Peach'), or createLiWithContent('Peach)?
    Semantics in CSS
       I don't understand this
       * "In CSS, consider styling a list with li elements representing different types of fruits. Would you know what part of the DOM is being selected with div > ul> li, or .fruits_item?

