# Font Properties CSS

In this lesson, we'll explore how to select and style fonts for your website. Fonts play a crucial role in web design, and your choice of fonts can significantly impact the overall look and feel of your site.

## Serif vs. Sans Serif Fonts

There are two major font categories: serif and sans-serif.

- **Serif Fonts:** Serif fonts have small decorative lines or "feet" at the ends of the letters. These fonts are often considered more traditional and formal. Examples of serif fonts include Times New Roman and Georgia.

- **Sans-serif Fonts:** Sans-serif fonts lack those decorative lines or "feet." They are often seen as modern and more straightforward. Examples of sans-serif fonts include Arial and Helvetica.

You can specify whether you want to use a serif or sans-serif font for your website by setting the `font-family` property in your CSS.

```css
/* Example of using a sans-serif font */
body {
    font-family: sans-serif;
}

/* Example of using a serif font */
body {
    font-family: serif;
}
```

## Using Web Safe Fonts

While you can choose any font for your website, it's important to consider web safe fonts. Web safe fonts are fonts that are widely available across various operating systems and browsers. Using web safe fonts helps ensure a consistent viewing experience for your website visitors.

Here are some commonly used web safe fonts:

- **Serif Fonts:** Georgia, Times New Roman
- **Sans-serif Fonts:** Arial, Helvetica, Comic Sans MS

You can create a font stack that includes multiple fonts in case the preferred font is not available on the user's system. This ensures that your design remains consistent. Here's an example of a font stack:

```css
body {
    font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
}
```

In this example, the browser will try to use "Helvetica Neue" first. If it's not available, it will attempt to use Helvetica, and if that's not available either, it will fall back to Arial. Finally, if none of these fonts are available, it will use a generic sans-serif font.

## Embedding Custom Fonts

If you want to use a specific font that's not available as a web safe font, you can embed custom fonts using services like Google Fonts. Here's how to do it:

1. Visit [Google Fonts](https://fonts.google.com/) and select the font(s) you want to use.
2. Click on the selected font(s) to open the font details.
3. Choose the styles (e.g., regular, bold, italic) you need.
4. Click the "Embed" tab to get the `<link>` tag to include in your HTML.

For example:

```html
<link href="https://fonts.googleapis.com/css2?family=Merriweather:ital,wght@0,400;0,700;1,400&display=swap" rel="stylesheet">
```

5. In your CSS, use the selected font by specifying its name:

```css
body {
    font-family: 'Merriweather', serif;
}
```

This code uses the "Merriweather" font as the primary font for the `body`, with `serif` as a fallback in case the font fails to load.
