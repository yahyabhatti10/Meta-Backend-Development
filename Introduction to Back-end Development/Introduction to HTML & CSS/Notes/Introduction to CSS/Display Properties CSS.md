# Display Properties CSS

In this lesson, we'll continue working on our website and focus on adding content and understanding CSS display properties. We'll also explore different display values and their effects on element positioning.

## Understanding CSS Display Properties

- ### Block Elements
Some HTML elements are considered block elements by default. These elements take up the entire width of the page and don't allow other elements to be on the same line to their left or right. Common block elements include headings (`h1` to `h6`), paragraphs (`p`), `div`, lists (`ul`, `ol`) and form elements.

- ### Inline Elements
Inline elements, on the other hand, only occupy the space they need in terms of height and width. They allow other elements to sit next to them horizontally. Common inline elements include `span`, `img`, and `a` (anchor) tags.

- ### Inline-Block Elements
The `inline-block` display property combines features of both block and inline elements. It allows you to set the width and height of the element while still allowing it to sit on the same line as other inline elements. This is often used for elements like images (`img`), which behave as inline-block by default.

- ### None Display
Setting an element's display property to `none` makes it disappear entirely from the webpage. It's as if the element was never part of the HTML structure.


## Styling and Hiding Elements

- **Styling Elements:** You can change the display property of an element to influence its behavior and position on the webpage. For example, changing `display: inline-block` allows you to set the width and height of inline elements.

- **Hiding Elements:** You can use `display: none` to completely remove an element from the webpage. Alternatively, the `visibility: hidden` property hides an element while maintaining its position in the layout.
