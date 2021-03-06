---
title: CSS3 Reference
author: Dan Hahn
date: 2/7/2018 15:00
template: single.jade
---

### Selectors
Selector|Example|Example description|CSS
---|---|---|---
.class|.intro|Selects all elements with class="intro"|1
#id|#firstname|Selects the element with id="firstname"|1
\*|\*|Selects all elements|2
element|p|Selects all <code>&lt;p&gt;</code> elements|1
element,element|div, p|Selects all <code>&lt;div> elements and all <code>&lt;p&gt;</code> elements|1
element element|div p|Selects all <code>&lt;p&gt;</code> elements inside <code>&lt;div> elements|1
element>element|div > p|Selects all <code>&lt;p&gt;</code> elements where the parent is a <code>&lt;div&gt;</code> element|2
element+element|div + p|Selects all <code>&lt;p&gt;</code> elements that are placed immediately after <code>&lt;div&gt;</code> elements|2
element1~element2|p ~ ul|Selects every <code>&lt;ul&gt;</code> element that are preceded by a <code>&lt;p&gt;</code> element|3
[attribute]|[target]|Selects all elements with a target attribute|2
[attribute=value]|[target=\_blank]|Selects all elements with target="\_blank"|2
[attribute~=value]|[title~=flower]|Selects all elements with a title attribute containing the word "flower"|2
[attribute&124;=value]|[lang&124;=en]|Selects all elements with a lang attribute value starting with "en"|2
[attribute^=value]|a[href^="https"]|Selects every <code>&lt;a&gt;</code> element whose href attribute value begins with "https"|3
[attribute$=value]|a[href$=".pdf"]|Selects every <code>&lt;a&gt;</code> element whose href attribute value ends with ".pdf"|3
[attribute*=value]|a[href*="w3schools"]|Selects every <code>&lt;a&gt;</code> element whose href attribute value contains the substring "w3schools"|3
:active|a:active|Selects the active link|1
::after|p::after|Insert something after the content of each <code>&lt;p&gt;</code> element|2
::before|p::before|Insert something before the content of each <code>&lt;p&gt;</code> element|2
:checked|input:checked|Selects every checked <code>&lt;input&gt;</code> element|3
:disabled|input:disabled|Selects every disabled <code>&lt;input&gt;</code> element|3
:empty|p:empty|Selects every <code>&lt;p&gt;</code> element that has no children (including text nodes)|3
:enabled|input:enabled|Selects every enabled <code>&lt;input&gt;</code> element|3
:first-child|p:first-child|Selects every <code>&lt;p&gt;</code> element that is the first child of its parent|2
::first-letter|p::first-letter|Selects the first letter of every <code>&lt;p&gt;</code> element|1
::first-line|p::first-line|Selects the first line of every <code>&lt;p&gt;</code> element|1
:first-of-type|p:first-of-type|Selects every <code>&lt;p&gt;</code> element that is the first <code>&lt;p&gt;</code> element of its parent|3
:focus|input:focus|Selects the input element which has focus|2
:hover|a:hover|Selects links on mouse over|1
:in-range|input:in-range|Selects input elements with a value within a specified range|3
:invalid|input:invalid|Selects all input elements with an invalid value|3
:lang(language)|p:lang(it)|Selects every <code>&lt;p&gt;</code> element with a lang attribute equal to "it" (Italian)|2
:last-child|p:last-child|Selects every <code>&lt;p&gt;</code> element that is the last child of its parent|3
:last-of-type|p:last-of-type|Selects every <code>&lt;p&gt;</code> element that is the last <code>&lt;p&gt;</code> element of its parent|3
:link|a:link|Selects all unvisited links|1
:not(selector)|:not(p)|Selects every element that is not a <code>&lt;p&gt;</code> element|3
:nth-child(n)|p:nth-child(2)|Selects every <code>&lt;p&gt;</code> element that is the second child of its parent|3
:nth-last-child(n)|p:nth-last-child(2)|Selects every <code>&lt;p&gt;</code> element that is the second child of its parent, counting from the last child|3
:nth-last-of-type(n)|p:nth-last-of-type(2)|Selects every <code>&lt;p&gt;</code> element that is the second <code>&lt;p&gt;</code> element of its parent, counting from the last child|3
:nth-of-type(n)|p:nth-of-type(2)|Selects every <code>&lt;p&gt;</code> element that is the second <code>&lt;p&gt;</code> element of its parent|3
:only-of-type|p:only-of-type|Selects every <code>&lt;p&gt;</code> element that is the only <code>&lt;p&gt;</code> element of its parent|3
:only-child|p:only-child|Selects every <code>&lt;p&gt;</code> element that is the only child of its parent|3
:optional|input:optional|Selects input elements with no "required" attribute|3
:out-of-range|input:out-of-range|Selects input elements with a value outside a specified range|3
:read-only|input:read-only|Selects input elements with the "readonly" attribute specified|3
:read-write|input:read-write|Selects input elements with the "readonly" attribute NOT specified|3
:required|input:required|Selects input elements with the "required" attribute specified|3
:root|:root|Selects the document's root element|3
::selection|::selection|Selects the portion of an element that is selected by a user| 
:target|#news:target |Selects the current active #news element (clicked on a URL containing that anchor name)|3
:valid|input:valid|Selects all input elements with a valid value|3
:visited|a:visited|Selects all visited links|1"

## Color Properties
Property|Description|CSS
---|---|---
color|Sets the color of text|1
| <code>color: color &#124; initial &#124; inherit;</code> |
opacity|Sets the opacity level for an element|3
|<code>opacity: number &#124; initial &#124; inherit;</code>|

## Background
Property|Description|CSS
---|---|---
background|A shorthand property for setting all the background properties in one declaration|1
|<code>background: bg-color bg-image position/bg-size bg-repeat bg-origin bg-clip bg-attachment initial &#124; inherit;</code>|
background-attachment|Sets whether a background image is fixed or scrolls with the rest of the page|1
|<code>background-attachment: scroll &#124; fixed &#124; local &#124; initial &#124; inherit;</code>|
background-blend-mode|Specifies the blending mode of each background layer (color/image)|3
|<code>background-blend-mode: normal &#124; multiply &#124; screen &#124; overlay &#124; darken &#124; lighten &#124; color-dodge &#124; saturation &#124; color &#124; luminosity;</code>|
background-color|Specifies the background color of an element|1
|<code>background-color: color &#124; transparent &#124; initial &#124; inherit;</code>|
background-image|Specifies one or more background images for an element|1
|<code>background-image: url &#124; none &#124; initial &#124; inherit;</code>|
background-position|Specifies the position of a background image|1
|<code>background-position: value;</code>|
background-repeat|Sets how a background image will be repeated|1
|<code>background-repeat: repeat &#124; repeat-x &#124; repeat-y &#124; no-repeat &#124; initial &#124; inherit;</code>|
background-clip|Specifies the painting area of the background|3
|<code>background-clip: border-box &#124; padding-box &#124; content-box &#124; initial &#124; inherit;</code>|
background-origin|Specifies where the background image(s) is/are positioned|3
|<code>background-origin: padding-box &#124; border-box &#124; content-box &#124; initial &#124; inherit;</code>|
background-size|Specifies the size of the background image(s)|3
|<code>background-size: auto &#124; length &#124; cover &#124; contain &#124; initial &#124; inherit;</code>|

## Border Properties
Property|Description|CSS
---|---|---
border|Sets all the border properties in one declaration|1
|<code>border: border-width border-style border-color &#124; initial &#124; inherit;</code>|
border-bottom|Sets all the bottom border properties in one declaration|1
|<code>border-bottom: border-width border-style border-color &#124; initial &#124; inherit;</code>|
border-bottom-color|Sets the color of the bottom border|1 
border-bottom-left-radius|Defines the shape of the border of the bottom-left corner|3
border-bottom-right-radius|Defines the shape of the border of the bottom-right corner|3
border-bottom-style|Sets the style of the bottom border|1
border-bottom-width|Sets the width of the bottom border|1
border-color|Sets the color of the four borders|1
|<code>border-color: color &#124; transparent &#124; initial &#124; inherit;</code>|
border-image|A shorthand property for setting all the border-image-* properties|3
|<code>border-image: source slice width outset repeat &#124; initial &#124; inherit;</code>|
border-image-outset|Specifies the amount by which the border image area extends beyond the border box|3
border-image-repeat|Specifies whether the border image should be repeated, rounded or stretched|3
border-image-slice|Specifies how to slice the border image|3
border-image-source|Specifies the path to the image to be used as a border|3
border-image-width|Specifies the widths of the image-border|3
border-left|Sets all the left border properties in one declaration|1
|<code>border-left: border-width border-style border-color &#124; initial &#124; inherit;</code>|
border-left-color|Sets the color of the left border|1
border-left-style|Sets the style of the left border|1
border-left-width|Sets the width of the left border|1
border-radius|A shorthand property for setting all the four border-\*-radius properties|3
|<code>border-radius: 1-4 length &#124; % / 1-4 length &#124; % &#124; initial &#124; inherit;</code>|
border-right|Sets all the right border properties in one declaration|1
|<code>border-right: border-width border-style border-color &#124; initial &#124; inherit;</code>|
border-right-color|Sets the color of the right border|1
border-right-style|Sets the style of the right border|1
border-right-width|Sets the width of the right border|1
border-style|Sets the style of the four borders|1
|<code>border-style: none &#124; hidden &#124; dotted &#124; dashed &#124; solid &#124; double &#124; groove &#124; ridge &#124; inset &#124; outset &#124; initial &#124; inherit;</code>|
border-top|Sets all the top border properties in one declaration|1
|<code>border-top: border-width border-style border-color &#124; initial &#124; inherit;</code>|
border-top-color|Sets the color of the top border|1
border-top-left-radius|Defines the shape of the border of the top-left corner|3
border-top-right-radius|Defines the shape of the border of the top-right corner|3
border-top-style|Sets the style of the top border|1
border-top-width|Sets the width of the top border|1
border-width|Sets the width of the four borders|1
|<code>border-width: medium &#124; thin &#124; thick &#124; length &#124; initial &#124; inherit;</code>|
box-decoration-break|Sets the behavior of the background and border of an element at page-break, or, for  in-line elements, at line-break.|3
box-shadow|Attaches one or more drop-shadows to the box|3
|<code>box-shadow: none &#124; h-shadow v-shadow blur spread color  &#124; inset &#124; initial &#124; inherit;</code>|

## Basic Box Properties

Property|Description|CSS
---|---|---
bottom|Specifies the bottom position of a positioned element|2
|<code>bottom: auto &#124; length &#124; initial &#124; inherit;</code>|
clear|Specifies which sides of an element where other floating elements are not allowed|1
|<code>clear: none &#124; left &#124; right &#124; both &#124; initial &#124; inherit;</code>|
clip|Clips an absolutely positioned element|2
|<code>clip: auto &#124; shape &#124; initial &#124; inherit;</code>|
display|Specifies how a certain HTML element should be displayed|1
|<code>display: inline &#124; block &#124; flex &#124; inline-block &#124; inline-flex &#124; inline-table &#124; list-item &#124; run-in &#124; table &#124; table-caption &#124;      table-column-group &#124; table-header-group &#124; table-footer-group &#124; table-row-group &#124; table-cell &#124; table-column &#124; table-row &#124; none &#124; initial &#124; inherit;</code>|
float|Specifies whether or not a box should float|1
|<code>float: none &#124; left &#124; right &#124; initial &#124; inherit;</code>|
height|Sets the height of an element|1
|<code>height: auto &#124; length &#124; initial &#124; inherit;</code>|
left|Specifies the left position of a positioned element|2
|<code>left: auto &#124; length &#124; initial &#124; inherit;</code>|
margin|Sets all the margin properties in one declaration|1
|<code>margin: length &#124; auto &#124; initial &#124; inherit;</code>|
margin-bottom|Sets the bottom margin of an element|1
margin-left|Sets the left margin of an element|1
margin-right|Sets the right margin of an element|1
margin-top|Sets the top margin of an element|1
max-height|Sets the maximum height of an element|2
|<code>max-height: none &#124; length &#124; initial &#124; inherit;</code>|
max-width|Sets the maximum width of an element|2
|<code>max-width: none &#124; length &#124; initial &#124; inherit;</code>|
min-height|Sets the minimum height of an element|2
|<code>min-height: none &#124; length &#124; initial &#124; inherit;</code>|
min-width|Sets the minimum width of an element|2
|<code>min-width: none &#124; length &#124; initial &#124; inherit;</code>|
overflow|Specifies what happens if content overflows an element's box|2
|<code>overflow: visible &#124; hidden &#124; scroll &#124; auto &#124; initial &#124; inherit;</code>|
overflow-x|Specifies whether or not to clip the left/right edges of the content, if it overflows the element's content area|3
|<code>overflow: visible &#124; hidden &#124; scroll &#124; auto &#124; initial &#124; inherit;</code>|
overflow-y|Specifies whether or not to clip the top/bottom edges of the content, if it overflows the element's content area|3
|<code>overflow: visible &#124; hidden &#124; scroll &#124; auto &#124; initial &#124; inherit;</code>|
padding|Sets all the padding properties in one declaration|1
|<code>padding: length &#124; initial &#124; inherit;</code>|
padding-bottom|Sets the bottom padding of an element|1
padding-left|Sets the left padding of an element|1
padding-right|Sets the right padding of an element|1
padding-top|Sets the top padding of an element|1
position|Specifies the type of positioning method used for an element (static, relative, absolute or fixed)|2
|<code>position: static &#124; absolute &#124; fixed &#124; relative &#124; initial &#124; inherit;</code>|
right|Specifies the right position of a positioned element|2
|<code>right:  auto &#124; length &#124; initial &#124; inherit;</code>|
top|Specifies the top position of a positioned element|2
|<code>top:  auto &#124; length &#124; initial &#124; inherit;</code>|
visibility|Specifies whether or not an element is visible|2
|<code>visibility: visible &#124; hidden &#124; collapse &#124; initial &#124; inherit;</code>|
width|Sets the width of an element|1
|<code>width: auto &#124; value &#124; initial &#124; inherit;</code>|
vertical-align|Sets the vertical alignment of an element|1
|<code>vertical-align: baseline &#124; length &#124; sub &#124; super &#124; top &#124; text-top &#124; middle &#124; bottom &#124; text-bottom &#124; initial &#124; inherit;</code>|
z-index|Sets the stack order of a positioned element|2
|<code>z-index: auto &#124; number &#124; initial &#124; inherit;</code>|

## Flexible Box Layout

Property|Description|CSS
---|---|---
align-content|Specifies the alignment between the lines inside a flexible container when the items do not use all available space|3
|<code>align-content: stretch &#124; center &#124; flex-start &#124; flex-end &#124; space-between &#124; space-around &#124; initial &#124; inherit;</code>|
align-items|Specifies the alignment for items inside a flexible container|3
|<code>align-items: stretch &#124; center &#124; flex-start &#124; flex-end &#124; baseline &#124; initial &#124; inherit;</code>|
align-self|Specifies the alignment for selected items inside a flexible container|3
|<code>align-self: auto &#124; stretch &#124; center &#124; flex-start &#124; flex-end &#124; baseline &#124; initial &#124; inherit;</code>|
flex|Specifies the length of the item, relative to the rest|3
|<code>flex: flex-grow flex-shrink flex-basis &#124; auto &#124; initial &#124; inherit;</code>|
flex-basis|Specifies the initial length of a flexible item|3
|<code>flex-basis: number &#124; auto &#124; initial &#124; inherit;</code>|
flex-direction|Specifies the direction of the flexible items|3
|<code>flex-direction: row &#124; row-reverse &#124; column &#124; column-reverse &#124; initial &#124; inherit;</code>|
flex-flow|A shorthand property for the flex-direction and the flex-wrap properties|3
|<code>flex-flow: flex-direction flex-wrap &#124; initial &#124; inherit;</code>|
flex-grow|Specifies how much the item will grow relative to the rest|3
|<code>flex-grow: number &#124; initial &#124; inherit;</code>|
flex-shrink|Specifies how the item will shrink relative to the rest|3
|<code>flex-shrink: number &#124; initial &#124; inherit;</code>|
flex-wrap|Specifies whether the flexible items should wrap or not|3
|<code>flex-wrap: nowrap &#124; wrap &#124; wrap-reverse &#124; initial &#124; inherit;</code>|
justify-content|Specifies the alignment between the items inside a flexible container when the items do not use all available space|3
|<code>justify-content: flex-start &#124; flex-end &#124; center &#124; space-between &#124; space-around &#124; initial &#124; inherit;</code>|
order|Sets the order of the flexible item, relative to the rest|3
|<code>order: number &#124; initial &#124; inherit;</code>|

## Text Properties
Property|Description|CSS
---|---|---
letter-spacing|Increases or decreases the space between characters in a text|1
|<code>letter-spacing: normal &#124; length &#124; initial &#124; inherit;</code>|
line-height|Sets the line height|1
|<code>line-height: normal &#124; number &#124; length &#124; initial &#124; inherit;</code>|
tab-size|Specifies the length of the tab-character|3
|<code>tab-size: number &#124; length &#124; initial &#124; inherit;</code>|
text-align|Specifies the horizontal alignment of text|1
|<code>text-align: left &#124; right &#124; center &#124; justify &#124; initial &#124; inherit;</code>|
text-align-last|Describes how the last line of a block or a line right before a forced line break is aligned when text-align is justify|3
|<code>text-align-last: auto &#124; left &#124; right &#124; center &#124; justify &#124; start &#124; end &#124; initial &#124; inherit;</code>|
text-decoration|Specifies the decoration added to text|1
|<code>text-decoration: none &#124; underline &#124; overline &#124; line-through &#124; initial &#124; inherit;</code>|
text-indent|Specifies the indentation of the first line in a text-block|1
|<code>text-indent: length &#124; initial &#124; inherit;</code>|
text-transform|Controls the capitalization of text|1
|<code>text-transform: none &#124; capitalize &#124; uppercase &#124; lowercase &#124; initial &#124; inherit;</code>|
white-space|Specifies how white-space inside an element is handled|1
|<code>white-space: normal &#124; nowrap &#124; pre &#124; pre-line &#124; pre-wrap &#124; initial &#124; inherit;</code>|
word-spacing|Increases or decreases the space between words in a text|1
|<code>word-spacing: normal &#124; length &#124; initial &#124; inherit;</code>|
word-wrap|Allows long, unbreakable words to be broken and wrap to the next line|3
|<code>word-wrap: normal &#124; break-word &#124; initial &#124; inherit;</code>|

## Font Properties
Property|Description|CSS
---|---|---
@font-face|A rule that allows websites to download and use fonts other than the web-safe fonts|3
font|Sets all the font properties in one declaration|1
|<code>font: font-style font-variant font-weight font-size/line-height font-family &#124; caption &#124; icon &#124; menu &#124; message-box &#124; small-caption &#124; status-bar &#124; initial &#124; inherit;</code>|
font-family|Specifies the font family for text|1
|<code>font-family: family-name &#124; generic-family &#124; initial &#124; inherit;</code>|
font-size|Specifies the font size of text|1
|<code>font-size:medium &#124; xx-small &#124; x-small &#124; small &#124; large &#124; x-large &#124; xx-large &#124; smaller &#124; larger &#124; length &#124; initial &#124; inherit;</code>|
font-style|Specifies the font style for text|1
|<code>font-style: normal &#124; italic &#124; oblique &#124; initial &#124; inherit;</code>|
font-variant|Specifies whether or not a text should be displayed in a small-caps font|1
|<code>font-variant: normal &#124; small-caps &#124; initial &#124; inherit;</code>|
font-weight|Specifies the weight of a font|1
|<code>font-weight: normal &#124; bold &#124; bolder &#124; lighter &#124; number &#124; initial &#124; inherit;</code>|

## Table Properties
Property|Description|CSS
---|---|---
border-collapse|Specifies whether or not table borders should be collapsed|2
|<code>border-collapse: separate &#124; collapse &#124; initial &#124; inherit;</code>|
border-spacing|Specifies the distance between the borders of adjacent cells|2
|<code>border-spacing: length &#124; initial &#124; inherit;</code>|
caption-side|Specifies the placement of a table caption|2
|<code>caption-side: top &#124; bottom &#124; initial &#124; inherit;</code>|
empty-cells|Specifies whether or not to display borders and background on empty cells in a table|2
|<code>empty-cells: show &#124; hide &#124; initial &#124; inherit;</code>|
table-layout|Sets the layout algorithm to be used for a table|2
|<code>table-layout: auto &#124; fixed &#124; initial &#124; inherit;</code>|

## Lists and Counters Properties
Property|Description|CSS
---|---|---
counter-increment|Increments one or more counters|2
|<code>counter-increment: none &#124; id &#124; initial &#124; inherit;</code>|
counter-reset|Creates or resets one or more counters|2
|<code>counter-reset: none &#124; name number &#124; initial &#124; inherit;</code>|
list-style|Sets all the properties for a list in one declaration|1
|<code> list-style: list-style-type list-style-position list-style-image &#124; initial &#124; inherit;</code>|
list-style-image|Specifies an image as the list-item marker|1
|<code>list-style-image: none &#124; url &#124; initial &#124; inherit;</code>|
list-style-position|Specifies if the list-item markers should appear inside or outside the content flow|1
|<code>list-style-position: inside &#124; outside &#124; initial &#124; inherit;</code>|
list-style-type|Specifies the type of list-item marker|1
|<code>list-style-type: disc &#124; armenian &#124; circle &#124; cjk-ideographic &#124; decimal &#124; decimal-leading-zero &#124; georgian &#124; hebrew &#124; hiragana &#124; hiragana-iroha &#124; katakana &#124; katakana-iroha &#124; lower-alpha &#124; lower-greek &#124; lower-latin &#124; lower-roman &#124; none &#124; square &#124; upper-alpha &#124; upper-greek &#124; upper-latin &#124; upper-roman &#124; initial &#124; inherit</code>|



## Animation Properties
Property|Description|CSS
---|---|---
@keyframes|Specifies the animation code|3
|<code>@keyframes animationname {keyframes-selector {css-styles;}}</code>|
animation|A shorthand property for all the animation properties (except animation-play-state and animation-fill-mode)|3
|<code>animation: name duration timing-function delay iteration-count direction fill-mode play-state;</code>|
animation-delay|Specifies a delay for the start of an animation|3
|<code>animation-delay: time &#124; initial &#124; inherit;</code>|
animation-direction|Specifies whether or not the animation should play in reverse on alternate cycles|3
|<code>animation-direction: normal &#124; reverse &#124; alternate &#124; alternate-reverse &#124; initial &#124; inherit;</code>|
animation-duration|Specifies how many seconds or milliseconds an animation takes to complete one cycle|3
|<code>animation-duration: time &#124; initial &#124; inherit;</code>|
animation-fill-mode|Specifies a style for the element when the animation is not playing (when it is finished, or when it has a delay)|3
|<code>animation-fill-mode: none &#124; forwards &#124; backwards &#124; both &#124; initial &#124; inherit;</code>|
animation-iteration-count|Specifies the number of times an animation should be played|3
|<code>animation-iteration-count: number &#124; infinite &#124; initial &#124; inherit;</code>|
animation-name|Specifies the name of the `@keyframes` animation|3
|<code>animation-name: keyframename &#124; none &#124; initial &#124; inherit;</code>|
animation-play-state|Specifies whether the animation is running or paused|3
|<code>animation-play-state: paused &#124; running &#124; initial &#124; inherit;</code>|
animation-timing-function|Specifies the speed curve of an animation|3
|<code>animation-timing-function: linear &#124; ease &#124; ease-in &#124; ease-out &#124; ease-in-out &#124; step-start &#124; step-end &#124; steps(int,start &#124; end) &#124; cubic-bezier(n,n,n,n) &#124; initial &#124; inherit;</code>|

## Transform Properties
Property|Description|CSS
---|---|---
backface-visibility|Defines whether or not an element should be visible when not facing the screen|3
|<code>backface-visibility: visible &#124; hidden &#124; initial &#124; inherit;</code>|
perspective|Specifies the perspective on how 3D elements are viewed|3
|<code>perspective: length &#124; none;</code>|
perspective-origin|Specifies the bottom position of 3D elements|3
|<code>perspective-origin: x-axis y-axis &#124; initial &#124; inherit;</code>|
transform|Applies a 2D or 3D transformation to an element|3
|<code>transform: none &#124; matrix(n,n,n,n,n,n) &#124; matrix3d (n,n,n,n,n,n,n,n,n,n,n,n,n,n,n,n) &#124; translate(x,y) &#124; translate3d(x,y,z) &#124; translateX(x) &#124; translateY(y) &#124; translateZ(z) &#124; scale(x,y) &#124; scale3d(x,y,z) &#124; scaleX(x) &#124; scaleY(y) &#124; scaleZ(z) &#124; rotate(angle) &#124; rotate3d(x,y,z,angle) &#124; rotateX(angle) &#124; rotateY(angle) &#124; rotateZ(angle) &#124; skew(x-angle,y-angle) &#124; skewX(angle) &#124; skewY(angle) &#124; perspective(n) &#124; initial &#124; inherit;</code>|
transform-origin|Allows you to change the position on transformed elements|3
|<code>transform-origin: x-axis y-axis z-axis &#124; initial &#124; inherit;</code>|
transform-style|Specifies how nested elements are rendered in 3D space|3
|<code>transform-style: flat &#124; preserve-3d &#124; initial &#124; inherit;</code>|
## Transitions Properties
Property|Description|CSS
---|---|---
transition|A shorthand property for setting the four transition properties|3
|<code>transition: property duration timing-function delay &#124; initial &#124; inherit;</code>|
transition-property|Specifies the name of the CSS property the transition effect is for|3
|<code>transition-property: none &#124; all &#124; property &#124; initial &#124; inherit;</code>|
transition-duration|Specifies how many seconds or milliseconds a transition effect takes to complete|3
|<code>transition-duration: time &#124; initial &#124; inherit;</code>|
transition-timing-function|Specifies the speed curve of the transition effect|3
|<code>transition-timing-function: linear &#124; ease &#124; ease-in &#124; ease-out &#124; ease-in-out &#124; step-start &#124; step-end &#124; steps(int,start &#124; end) &#124; cubic-bezier(n,n,n,n) &#124; initial &#124; inherit;</code>|
transition-delay|Specifies when the transition effect will start|3
|<code>transition-delay: time &#124; initial &#124; inherit;</code>|
## Basic User Interface Properties
Property|Description|CSS
---|---|---
box-sizing|Tells the browser what the sizing properties (width and height) should include|3
|<code>box-sizing: content-box &#124; border-box &#124; initial &#124; inherit;</code>|
cursor|Specifies the type of cursor to be displayed|2
|<code>cursor: alias &#124; all-scroll &#124; auto &#124; cell &#124; context-menu &#124; col-resize &#124; copy &#124; crosshair &#124; default &#124; e-resize &#124; ew-resize &#124; grab &#124; grabbing &#124; help &#124; move &#124; n-resize &#124; ne-resize &#124; nesw-resize &#124; ns-resize &#124; nw-resize &#124; nwse-resize &#124; no-drop &#124; none &#124; not-allowed &#124; pointer &#124; progress &#124; row-resize &#124; s-resize &#124; se-resize &#124; sw-resize &#124; text &#124; URL &#124; vertical-text &#124; w-resize &#124; wait &#124; zoom-in &#124; zoom-out &#124; initial &#124; inherit;</code>|
outline|Sets all the outline properties in one declaration|2
|<code>outline: outline-color outline-style outline-width &#124; initial &#124; inherit;</code>|
outline-color|Sets the color of an outline|2
|<code>outline-color: invert &#124; color &#124; initial &#124; inherit;</code>|
outline-offset|Offsets an outline, and draws it beyond the border edge|3
|<code>outline-offset: length &#124; initial &#124; inherit;</code>|
outline-style|Sets the style of an outline|2
|<code>outline-style: none &#124; hidden &#124; dotted &#124; dashed &#124; solid &#124; double &#124; groove &#124; ridge &#124; inset &#124; outset &#124; initial &#124; inherit;</code>|
outline-width|Sets the width of an outline|2
|<code>outline-width: medium &#124; thin &#124; thick &#124; length &#124; initial &#124; inherit;</code>|
resize|Specifies whether or not an element is resizable by the user|3
|<code>resize: none &#124; both &#124; horizontal &#124; vertical &#124; initial &#124; inherit;</code>|
text-overflow|Specifies what should happen when text overflows the containing element|3
|<code>text-overflow: clip &#124; ellipsis &#124; string &#124; initial &#124; inherit;</code>|
## Multi-column Layout Properties
Property|Description|CSS
---|---|---
column-count|Specifies the number of columns an element should be divided into|3
|<code>column-count: number &#124; auto &#124; initial &#124; inherit;</code>|
column-gap|Specifies the gap between the columns|3
|<code>column-gap: length &#124; normal &#124; initial &#124; inherit;</code>|
column-rule|A shorthand property for setting all the column-rule-* properties|3
|<code>column-rule: column-rule-width column-rule-style column-rule-color &#124; initial &#124; inherit;</code>|
column-rule-color|Specifies the color of the rule between columns|3
|<code>column-rule-color: color &#124; initial &#124; inherit;</code>|
column-rule-style|Specifies the style of the rule between columns|3
|<code>column-rule-style: none &#124; hidden &#124; dotted &#124; dashed &#124; solid &#124; double &#124; groove &#124; ridge &#124; inset &#124; outset &#124; initial &#124; inherit;</code>|
column-rule-width|Specifies the width of the rule between columns|3
|<code>column-rule-width: medium &#124; thin &#124; thick &#124; length &#124; initial &#124; inherit;</code>|
column-span|Specifies how many columns an element should span across|3
|<code>column-span: 1 &#124; all &#124; initial &#124; inherit;</code>|
column-width|Specifies the width of the columns|3
|<code>column-width: auto &#124; length &#124; initial &#124; inherit;</code>|
columns|A shorthand property for setting column-width and column-count|3
|<code>columns: auto &#124; column-width column-count &#124; initial &#124; inherit;</code>|

### Pseudo-Classes
Name|Applies to|Example
-|-|-
a:link|anchor|A:link, A.classname:link
a:active|anchor|A:active, A.classname:active
a:visited|anchor|A:visited, A.classname:visited
e:hover|all|P:hover, P.classname:hover

### Pseudo Elements
Pseudo-elements|Applies to
-|-|-
E:before|block
E:after|block
E:first-letter|block
E:first-line|block


### CSS Units

#### Absolute Lengths
The absolute length units are fixed and a length expressed in any of these will appear as exactly that size.

Absolute length units are not recommended for use on screen, because screen sizes vary so much. However, they can be used if the output medium is known, such as for print layout.

Unit|Description
-|-
cm|centimeters
mm|millimeters
in|inches (1in = 96px = 2.54cm)
px \*|pixels (1px = 1/96th of 1in)
pt|points (1pt = 1/72 of 1in)
pc|picas (1pc = 12 pt)

#### Relative Lengths
Relative length units specify a length relative to another length property. Relative length units scales better between different rendering mediums.

Unit|Description
-|-
em|Relative to the font-size of the element (2em means 2 times the size of the current font)
ex|Relative to the x-height of the current font (rarely used)
ch|Relative to width of the "0" (zero)
rem|Relative to font-size of the root element
vw|Relative to 1% of the width of the viewport*
vh|Relative to 1% of the height of the viewport*
vmin|Relative to 1% of viewport's* smaller dimension
vmax|Relative to 1% of viewport's* larger dimension
%|A percent of something

Note: Tip: The em and rem units are practical in creating perfectly scalable layout!
\* Viewport = the browser window size. If the viewport is 50cm wide, 1vw = 0.5cm.

### Colors
Unit|Description
-|-
color_name|A color name (red)
rgb(x,x,x)|A rgb value (rgb(255,0,0))
rgb(y%, y%, y%)|A rgb percentage value (rgb(100%,0%,0%))
#rrggbb|A hex number ( #ff0000).

<style>
table {width: 100%}
table tr td:first-of-type {white-space: nowrap;width: 20%;}
table tr td:nth-child(2) {width: 70%}
table:first-of-type tr td:nth-child(2) {width: auto}
table:first-of-type tr td:nth-child(3) {width: auto}
table tr td:nth-child(3) {width: 10%}
td {empty-cells: show}
</style>
