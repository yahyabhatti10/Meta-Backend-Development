# Introduction to Cascading Style Sheets (CSS)

## What is CSS?

CSS is a style sheet or style language, and its sole purpose is to style markup languages like HTML and XML. In this module, we'll explore the powerful capabilities of CSS that can transform your website from a 90s relic to a modern masterpiece.

## Why CSS Matters

Let's first grasp the significance of CSS and why it was created.

Back in the 90s, web developers were eager to enhance the appearance of their websites, but the available tools were quite limited. Visualizing what web design looked like in that era may not be pleasant, but the primary tool at their disposal was **HTML**.


To style their websites with HTML alone, developers had to rely on HTML tags. For instance, they used the `<font>` tag to change text fonts and tags like `<center>` to center elements on the screen.

Attributes were also used. For instance, changing the background color of an `<h1>` element involved using the `background-color` attribute with a specific color hex code.

However, complications arose when attempting to manipulate layouts solely with HTML. To achieve layouts where text and images appeared side by side, developers had to resort to using tables. The downside was that tables required copious amounts of code for even the simplest layouts.

Take a look at the extensive code needed for such a basic task:

```html
<table>
  <tr>
    <td>
      <img src="image.jpg" alt="Image">
    </td>
    <td>
      <h1>Your Heading</h1>
      <p>Your paragraphs go here.</p>
    </td>
  </tr>
</table>
```

Tables also posed problems such as syntax errors and debugging challenges. Complex layouts led to the nesting of tables within tables, creating messy and convoluted structures.

This is where **Cascading Style Sheets (CSS)** came to the rescue.

