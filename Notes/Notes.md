## Basic HTML and HTML5(structure of webpage to the browser.)

1. main (search engine and other developers find the main content of your page.), header, footer, nav, video, article, section .
2. img src alt, img element must have an alt attribute.
3. <a href>...</a> anchor text - destinated web adderess. anchor is used to create internal link. To create internal link to # plus the value of the id attribute.
<a href = "#contacts-header">Contacts</a> <!--- To add comment here --->
<h2 id = "contacts-header">Contacts</h2> <!--- target = "_blank" target attribute to open the next tab in browser--->
<target="_blank">
4. target and blank <p>
Here's a <a target="_blank" href="https://"> link to www.freecodecamp.org </a> for you to follow.
</p> <!---for dead link href = "#"--->
5. <ul>For making list<li>item 1</li> <li>item 2</li> </ul> ul = unordered list
6. <ol> For ordered list </ol>
7. <input type = "text", placeholder = "type of text here" required> <!---This is self closing tag for input, placeholder = text shown inside the search text, required param is for input feild required--->
8. <form action="/url-where-you-want-to-submit-form-data"><input></form>
9. Submit Button to a Form: <submit type="submit"> Submit</submit>
10. <label> <input type = "radio" name = "indoor-outdoor"> Indoor </label>
11. <label for="loving"><input id="loving" type="checkbox" name="personality"> Loving</label> <!---For checkbox param name should be same everywhere and type = checkbox here, param value = --->
12. <div> division element, purpose container for other elements.</div>
13. <! DOCTYPE html> <html> <!---THIS IS BASIC STRUCTURE---></html>
14. <! DOCTYPE html><html><head><meta /> <!---meta elements such as link, meta, title, style---> </head> <body><div></div></body></html>

<!---Basic HTML and HTML5--->


<!--- CSS Basics --->
## Basic CSS (CSS or Cascading Style Sheets, how to display the text and other content that you write in HTML. With, can control the color, font, size, spacing and other aspects of HTML elements.)

1. <h2, style = "color: red;"> ... </h2> <!---nust use ; at the end of styling--->
2. <style h2{ color: blue; }> </style>
3. CSS class declaration <style> .blue-text { color: blue;} </style> <!---css class blue text--->, can create by <h2 class="blue-text">Cats</h2>
4. <link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css"> <!---to import font-family--->
5. <img class="class1 class2"> <!---can apply multiple classes in class param---> 
6. <style>h2{order-radius: 10px; border-radius: 50%;} </style> <!---To manage corners--->
7. each elements also have an id attribute. 
8. Innside your style element, you always reference classes by putting a . in front of their names. You always reference ids by putting a # in front of their names.
9. Adjust the Padding of an Element: distance between border and text, increases by increasing padding.
10. An element's margin controls the amount of space between an element's border and surrounding elements. If you set the margin to a negative value, the element will grow larger.
11. CSS allows you to control the padding of all four individual sides of an element with th padding-top, padding-right, padding-bottom and padding-left properties.
12. Use Clockwise Notation to Specify the Padding/Margin of an Element, Padding : 10px 20px 10px 20px (top->right->bottom->left)
13. Absolute versus Relative Units: physical unit of length: mm, relative units : em or rem. 
14. !important is another method to overriding.
15. color: #F00, #F00F0A, instead of red,
16. To create CSS variable using --penguin-skin: gray;
17. background: var(--penguin-skin, black); set background black if your variable wasn't set. Note that this can be useful for debugging.
18. Improve Compatibility with Browser Fallbacks: When you create a variable, it is available for you to use inside the selector in which you create it.It also is available in any of that selector's descendants. This happens because CSS variables are inherited, just like ordinary properties. 
19. Use a media query to change a variable, 
20. :root{ --penguin-size: 300px; --penguin-skin: black} <!---is way to create variable---> and @media (max-width: 350px){: root{--penguin-size: 300px; --penguin-skin: black}} <!---apply its style whenever it is used--->


<!---Resposive Web Design--->
## Applied Visual Design (combination of typography, color theory, graphics, animation page layout, and more to help deliver you unique messag)

1. <strong>To make it bold</strong>, <em> for italic font style </em>, <s> having style text-decoration: line-through; </s>, <hr> Horizontal line.
2. box-shadow : offset-x, offset-y, blur-radius, spread-radius, color, box-shadow: 0 10px 20px rgba(0,0,0,0.19), 0, 6px, 6px, rbga(0,0,0,0.23)
3. The opacity property adjust the opacity, conversely and the transparency for an item.
4. text-transform : (lowercase, uppercase, capitalize, intial, inherit, none)
5. Hover State of an Achor Tag: a:hover{color: red;}
6. CSS treats each HTML element as its own box, CSS Box Model. The default layout of elements in this way is called the normal flow of a document, but CSS offers the position property to override it, when we set relative. 
7. Lock an Element to its Parent with Absolute Positioning: One nuance with absolute positioning is that it will be locked relative to its closest positioned ancetor. 
8. Key difference between the fixed and absolute positions is that an element with a fixed position won't move when the user scrolls.
9. Push elements left or right with the float property.
10. Change the position of overlapping elements with the z-index property: When elements are positioned to overlap( using position: absolute | relative | fixed | sticky), the element coming later in the HTML markup will, by default, appear on the top of the other elements.
11. another positioning technique is to center a block element horizontally. one way to do this is to set its margin : auto; This method works for images, too. Images are inline elements by default, but can be changed to block elements when you set the display: block;
12. The color wheel is a useful tool to visualize how colors relate to each other - it's circle where similat hues are neighbors and different hues are farther apart. when two colors are opposite each other on the wheel, they are called complementary colors. When placed side-by-side, these color appear more vibrant and produce strong visual contrast. 
Complementary colors:
red (#FF0000) and cyan (#00FFFF)
green (#00FF00) and magenta (#FF00FF)
blue (#0000ff) and yellow (#FFFF00)
13. Red, Green and Blue are called primary colors. mixing two primary colors created the secondary colors cyan (G + B), magenta (R + B). These secondary colors happen to be complement to the primary color not used in their creation, and are opposite to that primary color on the color wheel. Tertiary colors are the result of combining primary color with one of its secondary color neighbors. Ex: Red(Primary) and yellow(secondary) and make orange (tertiary).
14. Colors have several characteristics including hue, saturation, and lightness.CSS3 introduced the hsl() property as an alternative way, hue, saturation, Lightness. hue uses a color wheel concept(0-360), saturation(100% being fully saturated), and Lightness 0% (black) to 100%(white), where 50% is the normal color. red : hsl(0, 100%, 50%) yellow(60, 100%, 50%)
15. color gradient: background: linear-gradient(gradient_direction, color 1, color 2, color 3, ...);
16. Transform: scale(), to change the scale of an element, transform property has variety of functions that let you scale, move, rotate, skew, etc., your elements. When used with pseudo-classes such as :hover that specify a certain state of an elements, the transform property can easily add interactivity to your elements.
17. transform property is skewX() which skews the selected element along its X(horizontal) axis by a given degree. 
18. Create a graphic using CSS: ::before creates a pseudo-element that is the first child of the selected element; ::after created a pseudo-element that is the last child of the selected element. 
19. @keyframes and animation properties work, @keyframes twinkle {} rule. there are 8 animation properties.
20. In CSS animations, the animation-timing-function property controls how quickly an animated element changes over the duration of the animation. 
21. Bezier curves are used with the cubic-bezier function. The shape of the curve represents how the animation plays out. The curve lives on a 1 by 1 coordinate system. The X-axis of this coordinate system is the duratin of the animation(think of it as a time scale) and Y-axis is the change in the animation. 

<!---Applied Accessibility--->

1. Text Alternative to Images for Visually Impaired Accessibility:- 


4. data visulizations like charts, the caption can be used to briefly note the trends or conclusions for users with visual impairments
5. can improve form using <fieldset> <legend></legend><input id="",type="", name="", value=""><label></label></fieldset> can pick date by type="date". 
6. <input>has attribute type, name and value</input> 
7. <p>Master Camper Cat officiated the cage match between Goro and Scorpion <time datetime="2013-02-13">last Wednesday</time>, which ended in a draw.</p>
8. Make Elements Only Visible to a Screen Reader by Using Custom CSS, 
9. Avoid Colorblindness Issue by using sufficient Contrast- The WCAG-recommended contrast ratio of 4.5:1 applies for color use as well as gray-scale combinations.
10. tab index = 0, and focus attribute for pseudo class.
11. 

<!--- Resposive Web Design Principles --->

(How to use CSS to make your webpages look good, no matter what device they're viewed on)
1. Create a Media Query- Media Queries consist of a media type, and if that media type matches the type of device the document is displayed on, the styles are applied. You can have as man selectors and styles inside your media query as you want. 
2. @media() {rules}
3. Add the style rules to the responsive-img class.
4. Pixel Per Inch(PPI) or Dots Per Inch(DPI), display such "Retina Display" on the latest Apple MacBook Pro., instead of using em or px to size text, you can use viewport units for responsive typography. 
5. vw (viewport width): 10vw would be 10% of the viewport's width, vh (viewport height): 3vh would be 3% of the viewport's height, vmin(viewport minimum): 70vmin would be 70% of the viewport's smaller dimension (height or width), vmax( maximum): 100vmax would be 100% of the viewport's bigger dimension(height or width).

<!--- CSS Flexbox --->

(With flexbox, it's easy to center elements on the page and create dynamic user interfaces that shrink and expand automatically.)
(fundamentals of flexbox and dynamic layout by building a Twitter card.)
1. display : flex; flex-direction: row-reverse/column-reverse; 





<!--- CSS Grid --->
(newer standard grid that makes it easy to build complex responsive layouts. Fundamental of CSS grids by building diffirent complex layouts, including blogs.)
1. 