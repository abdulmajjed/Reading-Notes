Read: 06 - Design web pages with CSS.

#Introduce you to how CSS works
imagine that there is an invisible box around 
every HTML element.
allows you to create rules that control the 
way that each individual box

#Teach you how to write CSS rules
CSS rule contains two parts: a selector and a declaration
      selector    --->     p 
      declaration --->        font-family: Arial;

1.This rule indicates that all < p>elements should be shown in the Arial typeface. 
2.Selectors indicate which element the rule applies to. The same rule can apply to more than one element if you separate the element names with commas.
3.Declarations indicate how the elements referred to in the selector should be styled. Declarations are split into two parts a property and a value, and are separated by a colon.

two parts: a property and a value
h1, h2, h3 
               font-family: Arial;
                  color: yellow;
              property : value
*Properties indicate the aspects of the element you want to change. For example, color, font, width, height and border.
*Values specify the settings you want to use for the chosen properties

body 
 font-family: arial;
 background-color: rgb185,179,175;
h1 
 color: rgb255,255,255;

#Show you how CSS rules apply to HTML pages
< style>  include CSS within an HTML page by placing them inside a < style> element which usually sits inside the < head> element of the page

**CSS Selectors.

Universal Selector                          Targets all elements on the page
Type Selector                h1, h2, h3       Targets the < h1>, < h2> and  < h 3> elements
Class Selector               .note           Targets any element whose class attribute has a value of note
                             p.note         Targets only < p> elements   whose class attribute has a value of note
ID Selector                  #introduction    Targets the element whose id attribute has a value of introduction
Child Selector               li>a            Targets any < a> elements that are children of an  < li> element but not other < a> elements in the page
Descendant Selector          p a             Targets any < a> elements that sit inside a < p> element, even if there are other elements nested between them
Adjacent Sibling             h1+p           Targets the first < p> element after any < h1> element but not other < p> elements
Selector
General Sibling              h1~p            If you had two < p> elements that are siblings of an < h1> element, this rule would apply to bothSelector
 ------
#Chapter 11: Color
< head>
 < title>Color</ title>
 < style type="text/css">


CSS3: Opacity
opacity, rgba

p.one
background-color: rgb0,0,0;
opacity: 0.5;
p.two 
background-color: rgb0,0,0;
background-color: rgba0,0,0,0.5;

CSS3: HSL & HSLA
hsl, hsla
body 
background-color: #C8C8C8;
background-color: hsl0,0%,78%;
p 
background-color: #ffffff;
background-color: hsla0,100%,100%,0.5


