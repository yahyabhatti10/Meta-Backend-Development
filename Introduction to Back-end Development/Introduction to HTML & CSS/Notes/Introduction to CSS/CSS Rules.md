# CSS Rules
The precedence of CSS rules is determined as follows:

- **Importance**: Rules with `!important` declarations.

- **Type**: External CSS (linked stylesheet), internal CSS (within `<style>`), and inline styles.

- **Specificity**: Based on the number and type of selectors.

- **Position**: The order of rules in the stylesheet. 

Let's break down the provided CSS rules based on their precedence, starting from the highest precedence to the lowest:

### 1. **Importance (Highest Precedence)**:
---

CSS rules with the `!important` declaration have the highest precedence. They override any conflicting styles, regardless of specificity or type or position.

```css
color: red; /* This style is overridden */
color: green !important; /* This style takes precedence due to !important */
```

In this example, the `color: green !important;` rule will take precedence over the previous `color: red;` rule because of the `!important` declaration.

### 2. **Type (Second Precedence)**:
---

The type of CSS rules refers to where they are defined and their origin.

CSS rules have different origins or types. The order of precedence for these types, from highest to lowest, is as follows:

- **Inline Styles:** Styles defined directly in HTML elements using the style attribute. They have the highest precedence, and in the provided example, an inline style can override external or internal styles for the `<h1>` element.

- **Internal Styles:** Styles defined within the `<style>` tags in the `HTML` document. These apply to the entire document and have precedence over external styles.

- **External Styles:** Styles defined in an external CSS file (e.g., style.css) linked to the HTML document. These are applied after internal and inline styles.

```css
<link rel="stylesheet" href="./style.css"> <!-- External -->
<style> </style> <!-- Internal -->
<h1 style=" ">Hello</h1> <!-- Inline -->
```


### 3. **Specificity (Third Precedence)**:
---

Specificity determines which CSS rule takes precedence when multiple rules target the same element. It is calculated based on the number and type of selectors used.

- **IDs:** Selectors with ID attributes have the highest specificity and take precedence over other selectors.

- **Attributes:** Selectors with attribute take precedence over class and elements selectors.

- **Classes:** Selectors with Class come next in precedence and take precedence on elements selectors.

- **Elements:** Selectors targeting HTML elements without any additional attributes or classes have the lowest specificity and are overridden by more specific selectors.


```css
li { color: blue; } /* Element (4th precedence in Specificity) */
.first-class { color: red; } /* Class (3rd precedence in Specificity) */
li[draggable] { color: purple; } /* Attribute (2nd precedence in Specificity) */
#first-id { color: orange; } /* ID (1st precedence in Specificity) */
```

In a conflict between these rules targeting the same element, specificity is used to determine the final style.

### 4. **Position (Lowest Precedence)**:
---

CSS rules are cascading, meaning that if multiple rules target the same element and property, the last rule applied takes precedence. 

```css
li {
  color: red; /* Will be overridden */
  color: blue; /* Precedence because it's written later */
}
```




