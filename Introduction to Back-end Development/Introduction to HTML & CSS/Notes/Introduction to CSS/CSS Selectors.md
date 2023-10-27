# CSS Selectors

CSS (Cascading Style Sheets) selectors are used to target and style specific elements in an HTML document. Understanding the different types of selectors is essential for effectively styling web pages.

- **Universal Selector**
- **Type (Tag) Selector**
- **Class Selector**
- **ID Selector**

## 1. Universal Selector

The universal selector, denoted by an asterisk (*), selects all HTML elements on the page. It can be used to apply styles globally.

```css
* {
  margin: 0;
  padding: 0;
}
```

## 2. Type (Tag) Selector

The type selector targets all elements of a specific HTML tag. For example, to style all `<p>` elements:

```css
p {
  font-size: 16px;
}
```

## 3. Class Selector

The class selector targets elements with a specific `class` attribute. It allows you to style multiple elements with the same class.

```html
<p class="highlight">This is a highlighted paragraph.</p>
```

```css
.highlight {
  background-color: yellow;
}
```

## 4. ID Selector

The ID selector targets a single element with a unique `id` attribute. IDs should be unique within an HTML document.

```html
<div id="header">This is the header</div>
```

```css
#header {
  font-size: 24px;
}
```