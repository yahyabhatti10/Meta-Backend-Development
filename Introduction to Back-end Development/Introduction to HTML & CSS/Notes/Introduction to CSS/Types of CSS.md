# Types of CSS

**Cascading Style Sheets** (CSS) is used to style and format web documents. CSS can be applied in three different ways, each with its own use cases and advantages.

- **Inline CSS**
- **Internal CSS**
- **External CSS**

## 1. Inline CSS

Inline CSS is applied directly within an HTML element using the `style` attribute. It is useful for applying unique styles to individual HTML elements.

### Implementation:

```html
<p style="color: red; font-size: 18px;">This is a red and larger-sized text.</p>
```

In this example, the `style` attribute is used within the `<p>` tag to set the text color to red and the font size to 18 pixels.

## 2. Internal CSS

Internal CSS is defined within the HTML document using the `<style>` tag in the document's `<head>`. It is suitable for applying styles to multiple elements within the same page.

### Implementation:

```html
<!DOCTYPE html>
<html>
<head>
  <style>
    h1 {
      color: blue;
      font-size: 24px;
    }
    p {
      color: green;
      font-size: 16px;
    }
  </style>
</head>
<body>
  <h1>This is a blue, large heading.</h1>
  <p>This is a green, standard-sized paragraph.</p>
</body>
</html>
```

In this example, styles for both `<h1>` and `<p>` elements are defined within a `<style>` block in the document's `<head>`. These styles will be applied to all matching elements on the page.

## 3. External CSS

External CSS is stored in a separate `.css` file and linked to the HTML document using the `<link>` tag. It is the preferred method for applying styles consistently across multiple pages of a website.

### Implementation:

Create an external CSS file (e.g., `styles.css`):

```css
/* styles.css */
h1 {
  color: navy;
  font-size: 28px;
}

p {
  color: darkolivegreen;
  font-size: 18px;
}
```

Link the external CSS file in the HTML document:

```html
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
  <h1>This is a navy, large heading.</h1>
  <p>This is a dark olive green, medium-sized paragraph.</p>
</body>
</html>
```

In this example, an external CSS file (`styles.css`) defines styles for `<h1>` and `<p>` elements. The HTML document links to this external file using the `<link>` tag.

---

These are the three primary ways to apply CSS to HTML documents: Inline CSS, Internal CSS, and External CSS. Each method serves different purposes and offers flexibility in styling web content.