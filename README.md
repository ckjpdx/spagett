# Spagett's Pastas
Webpage for demonstrating floats, tables, CSS reset, pseudo elements and classes, positioning, alignment, and box model mechanics.

_by Chris Knight Johnson_

## CSS Used:
| CSS Code | DESCRIPTION | IMPLEMENTATION |
| - | - | - |
| Box-Sizing | This property determines how the element size is calculated. By default it is set to make calculations based on the outer most parts of the content area. This can cause sizing issues when padding or margin are added. | By setting this to border-box instead of content-box the elements can have margin and padding adjusted without it changing how much total space it occupies; the content will shrink to accommodate the changes instead of pushing out into other elements. Setting this to all elements is standard practice for most css files, or can be done manually using the asterisk selector. |
| Float | This property takes an element out of the normal flow of its containing element without removing it from the flow entirely. | Float was used to stack gallery images horizontally next to each other, space permitting. Float was also applied to the image of plain spaghetti in the text area so that the 2nd paragraph of text flows around the image while the image sits inside the paragraph's box model. |
| Display: Block | Sets an element to occupy an entire horizontal space, pushing any other non-floated or specially placed elements that would appear next to it down in the document flow. | Block was assigned to the Spagett hand icon in order to center the element and also act as an area of negative space between the upper and lower sections of the page |
| Display: Inline | Sets and element to wrap like text. Instead of taking up all horizontal space by insisting its has no neighbor elements to the left or right, inline will share a space with other inline elements and appear in the line according to where they are positioned in the DOM. | Inline display type was used to make list items that normally appear as blocks move next to each other like a sentence. This is a common way to make a nav bar of links at the top. |
| Centered Content | Block elements can be centered in their parent container by setting their margins to auto and inline elements by setting the parent container to text-align: center. | The footer paragraph was set to the inline setting text-align center. Also, the Spagett hand icon in the middle of the page was set to have its margins auto, having a similar effect. |
| Pseudo-Element | An element that doesn't exist in the HTML source code, but instead is added to the DOM by the CSS. | Background images were added before each paragraph in the main area of the page that displayed a "sauce bullet". |
| Pseudo-Class | An class styling that isn't applied to the DOM unless a specific condition is met, usually triggered by the user. | The effect :hover was added to the gallery images so that the box-shadow color turns white when the mouse is positioned over it. |
| Clear-Fix | A styling that is applied to impede the effect of floated elements from going any further down the DOM. | The footer section was given a clear fix class to prevent the floated gallery images from forcing the footer text over to the upper right, the last place the normal document flow existed before the float was applied. |
| Positional Selector | A CSS selector that chooses elements depending on their order in the DOM. | A different color background was applied to every other table row using the nth-child selector. |
| Selector Combinator | A CSS selector that chooses elements in relation to other elements, and increases that CSS rule's specificity. | A selection was made with "section.col-half.text-side img#speghetti-pile" which selected the image with the "id" of "speghetti-pile" that was nested in a section element that had both "classes" of "col-half" and "text-side". |

## Installation
Download via git by cloning and open in editor or download zip and open with an internet browser.

## Bugs
The footer doesn't inherit the font styles assigned with the * selector at the top of the CSS file and instead remains "serif". This is odd because a CSS reset is applied and no other rules change font-family to "serif". All other text seems to inherit the asterisk selector rule to change to "sans-serif". Applying a font-family rule by directly selecting the footer element will work.

## License
Open Source
