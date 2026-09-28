# Lab 2 - CSS Styling and Layouts

## File Organization
* `index.html`: Contains the core semantic HTML structure with 6 box elements (A through F).
* `styleA.css`: Implements a vertical layout using CSS Flexbox with dynamic equidistant spacing, horizontal centering, alternating row colors, and specific borders.
* `styleB.css`: Implements a horizontal inline layout with wrapping disabled, fixed viewport pinning for box F, dotted left borders, and custom hover states.

## Challenges Faced
* **Dynamic Vertical Distribution in Style A:** Ensuring boxes spaced themselves equally across the entire viewport without collapsing or distorting on window resize was solved by using `min-height: 100vh`, `justify-content: space-between`, and setting `flex-shrink: 0`.
* **Vertical Text Centering for Box F:** Centering text vertically within the final box in Style A while respecting the 4px border was handled cleanly via nested flex properties.
* **Separating Flow vs. Pinned Elements in Style B:** Keeping boxes A through E on a single non-wrapping line while anchoring box F to the bottom-right corner regardless of scrolling/resizing was solved using `white-space: nowrap` and `position: fixed`.
