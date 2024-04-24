# Lab Week 3 - CSS and Agile Intro
https://realized.me/sp24-cse110-lab3

## TODO:

### Global
- [x] External CSS stylesheet (preferred method for better code readability)
- [ ] Inline CSS (helpful for debugging)
- [x] Internal CSS with `<style>` (convenient for quick experiments)

### 1. General CSS Topics
-   ~~Comment /* write down comments to make your css easier to read */~~
-   Color                                               /* apply colors to your HTML elements */
    -   rgb(r, g, b) or rgba(r, g, b, a)     /* red, green, blue, alpha values */
    -   #FFF or #FFFFFF                    /* hex codes */
    -   hsl(h, s, l) or hsla(h, s, l, a)       /* hue, saturation, lightness, alpha values */
    -   ~~Color name (i.e 'orange')~~
    -   Wider-gamut color:
        -   color(colorspace c1 c2 c3[ / A])     /* predefined color space, values for color space*/
        -   color-mix(method, color1[ p1], color2[ p2])   /*method to mix colors, values & percentages of color*/
-   ~~CSS Variables & Fallbacks~~
    -   ~~Show at least one example of using a CSS variable that also has a fallback.~~

-   ~~[Background    Links to an external site.](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Backgrounds_and_borders#styling_backgrounds_in_css)/* apply background styles to your elements */~~

-   ~~background-color~~

-   [UnitLinks to an external site.](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Values_and_units)     /* units of measurement for sizing and spacing your elements */

-   Use 3 unique relative units total

-   Use 3 unique absolute units total

-   [Box ModelLinks to an external site.](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model)     /* configure the containers that holds your HTML content */\
    ("long" and "short" refer to longhand and shorthand syntax and should give the same results. They're simply different ways to declare your style rules, use at least one of each syntax. Y**ou must use both long and short hand notations for each of the following: margin, padding, border**) 

-   -   Margin     /* spacing between html elements */
        -   Long (margin-top, margin-bottom, margin-left, margin-right)
        -   Short (margin: <top> <right> <bottom> <left>)
        -   Auto margins: margin: auto
-   -   Padding     /* spacing within html elements */
        -   Long (padding-top, padding-bottom, padding-left, padding-right)
        -   Short (padding: <top> <right> <bottom> <left>)
-   -   [BordersLinks to an external site.](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Backgrounds_and_borders#borders)     /* borders around html elements, hint: apply borders before testing out padding and margin to better understand the difference between the two */
        -   border-style
        -   border-color
        -   border-width
        -   border-radius

-   Text     /* style your text */
    -   color
    -   text-decoration
    -   text-align

-   [DisplayLinks to an external site.](https://developer.mozilla.org/en-US/docs/Web/CSS/display)
    -   Experiment with these values: none, block, inline-block, inline. Include at least two of them in your page.
    -   Apply these values to the display property
-   Sizing     /* set the height and width for an element */

    -   height
    -   width
    -   max-width
    -   min-width    
-   [PositionLinks to an external site.](https://developer.mozilla.org/en-US/docs/Web/CSS/position)     /* element positioning on the page */
    -   2 of the following values: static, relative, fixed, absolute, sticky
        -   Apply these values to the position property
-   [Pseudo-classLinks to an external site.](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes)     /* elements that exist in your document conditionally */
    -   :hover
    -   :active
-   Layouts
    -   -   [FlexboxLinks to an external site.](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)   /* allow your elements to lay themselves out automatically */
            -   apply flex to the display property
            -   Must have more than two children within the element that is using flexbox. Must use minimum three of the flexbox related attributes
        -   [Grid Links to an external site.](https://css-tricks.com/snippets/css/complete-guide-grid/)        /* instantiate a grid for your layouts */
            -   apply grid to the display property
            -   Must have more than two children within the element that is using the grid. Must use a minimum of three of the grid related attributes
-   Responsiveness       /* make your website friendly for multiple devices */
    -   At least one query based on the screen width
        -   [Media QueryLinks to an external site.](https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries)
    -   Check the DevTools in your browser! Make sure your site works and looks fine on the three main types of form factors (Very small screen (phone), tablet or smaller laptop, and desktop).
    -   The layout of your page should automatically reflow when the size changes, meaning, we shouldn't have to pinch and zoom in a lot to read text, click buttons, etc.
-   [FontsLinks to an external site.](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Web_fonts)       /* pick varying font styles to make your text fun to read */
    -   Include and use a 3rd party font ([https://fonts.google.com/Links to an external site.](https://fonts.google.com/)). You can load the font in either your HTML or your CSS

### 2. CSS Selectors
CSS selectors allow you to select the HTML element you want to style. Each type of selector targets a different identifier on your HTML element. For this lab you must use at least one of every bulleted selector method.

-   Class Selector (.class)
-   ID Selector (#id)
-   Universal Selector (*)
-   Element Selector (element) 
-   Attribute Selector (e.g. [attribute=foo])

-   Pseudo-class Selector (e.g. p:hover)
-   Selector List (element, element)                   /* select multiple elements */

-   Combinators (you must use one of each)    /* specify selections based on element positioning in the DOM tree */

    -   Descendant Combinator (element element)
    -   Child Combinator (element > element)
    -   General sibling combinator (element ~ element)
    -   Adjacent sibling combinator (element + element)
    -   Combining Two Selectors (element.class)
-   New Selectors /*Adopted in December 2023!*/
    -   :has()  /*You must use this selector. Click [hereLinks to an external site.](https://developer.mozilla.org/en-US/docs/Web/CSS/:has "Link") for how to use. This is a new selector that was widely adopted in 2023.*/
    -   Nested Selectors
        -   Nested selectors are another type of selector that have recently been adopted in 2023. [HereLinks to an external site.](https://developer.mozilla.org/en-US/docs/Web/CSS/Nesting_selector "Link") is some more information about this selector. Please also include at least one type of this selector in your CSS.

### 3. CSS Validation
Similar to Lab 2, where we validated our HTML, we can also validate our CSS. Validate your CSS through a [validatorLinks to an external site.](https://jigsaw.w3.org/css-validator/ "Link") and take a screenshot. Add this screenshot to your repo! You might notice that the validator will throw an error for some of the newer selectors you used. If this is the case, that's ok!