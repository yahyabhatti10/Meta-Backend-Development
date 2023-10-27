# CSS Media Queries

CSS Media Queries allow you to apply different styles to your web page based on various device characteristics such as screen width, height, device orientation, and more. This documentation will guide you through the basics of using media queries in your CSS.



## Introduction

Media queries are a crucial part of responsive web design, enabling you to create layouts that adapt to different screen sizes and devices. By defining specific conditions in your CSS, you can control how your web page appears on various devices.

## Syntax

A media query in CSS typically follows this basic syntax:

```css
@media media-type and (media-feature) {
  /* CSS rules to apply when the media query matches */
}
```

- `@media`: This keyword indicates the start of a media query.
- `media-type`: Specifies the type of media, such as `screen`, `print`, `speech`, etc.
- `media-feature`: Defines the conditions under which the styles should be applied.
- CSS rules: The styles enclosed within the curly braces `{}` are applied when the media query's conditions are met.

## Media Features

Media features are conditions or criteria that you can use in media queries. Here are some common media features:

- **Width and Height**: 
  - `width`: Specifies the viewport's width.
  - `height`: Specifies the viewport's height.

- **Device Orientation**:
  - `orientation`: Checks the device's orientation, either `landscape` or `portrait`.

- **Resolution**:
  - `resolution`: Checks the screen's resolution, in DPI (dots per inch).

- **Device Type**:
  - `screen`: Used for screens and monitors.
  - `print`: Used for print devices.
  - `speech`: Used for screen readers and other speech synthesis devices.

- **Viewport Size**:
  - `min-width` and `max-width`: Defines a range of widths.
  - `min-height` and `max-height`: Defines a range of heights.

- **Color**:
  - `color`: Checks the number of bits per color component.
  - `color-index`: Checks the number of colors the device can display.

- **Aspect Ratio**:
  - `aspect-ratio`: Compares the width and height of the viewport.

- **Hover**:
  - `hover`: Detects if the device has a hover-capable pointing device.

- **Pointer Type**:
  - `pointer`: Detects the type of pointing device (e.g., mouse, touch).

- **Feature Queries**:
  - `@supports`: Tests whether a CSS feature is supported by the browser.

## Using Media Queries

To use media queries effectively, follow these steps:

1. Define the media query using the `@media` rule.
2. Specify the media type and one or more media features.
3. Inside the curly braces, add the CSS rules you want to apply when the conditions are met.

```css
@media screen and (max-width: 768px) {
  /* CSS rules for screens with a max width of 768px */
}
```

## Common Use Cases

1. **Responsive Layouts**: Adjust the layout of your website for different screen sizes.

2. **High-Resolution Graphics**: Serve high-resolution images on devices with high DPI screens.

3. **Print Stylesheets**: Create styles specifically for print media.

4. **Accessibility**: Modify styles for users with disabilities using screen readers.

5. **Interactive Elements**: Change styles when the device supports hover or touch events.

## Examples

### Example 1: Responsive Typography

```css
@media screen and (max-width: 768px) {
  body {
    font-size: 16px;
  }
}
```

### Example 2: High-Resolution Images

```css
@media screen and (min-resolution: 300dpi) {
  img {
    max-width: 100%;
    height: auto;
  }
}
```

## Best Practices

1. **Mobile-First Design**: Start with styles for mobile devices and progressively enhance for larger screens.

2. **Use Logical Operators**: Combine multiple media features with `and`, `not`, or `only` to create complex conditions.

3. **Test Thoroughly**: Test your media queries on various devices and browsers to ensure compatibility.

4. **Maintain Readability**: Keep your CSS organized and well-commented for easier maintenance.

5. **Avoid Overly Specific Queries**: Write media queries that are as generic as possible to accommodate various devices.

By understanding and utilizing CSS Media Queries, you can create responsive and user-friendly web designs that adapt to different devices and screen sizes.

For more information, refer to the [W3C CSS Media Queries Specification](https://www.w3.org/TR/css3-mediaqueries/).