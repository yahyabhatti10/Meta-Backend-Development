# Anatomy of HTML Tags and Elements

In this section, we'll break down the components of HTML tags and elements to understand their structure and usage.

## HTML Elements with Opening and Closing Tags

HTML elements consist of opening and closing tags, encasing content that should be structured. This concept resembles marking a manuscript for formatting in the publishing industry.

For example, consider the following HTML element:

```html
<p>Hello World</p>
```

In this case, `<p>` is the opening tag, and `</p>` is the closing tag. The content, "Hello World," falls between these tags, indicating how the browser should display it.

## Self-Closing HTML Tags

Some HTML tags are self-closing, meaning they don't require a separate closing tag. They are expressed like this:

```html
<br>
```

An example is the `<br>` tag, which represents a line break. Self-closing tags enhance the structure and layout of HTML documents without the need for closing counterparts.

## Using HTML Attributes

HTML elements can have attributes that provide additional information to the browser, modifying the element's default behavior. Attributes appear within the opening tag, separated by spaces.

For instance, the `<hr>` tag can take attributes like `size` and `noshade` to customize its appearance. The `size` attribute adjusts the height, while `noshade` removes shading. These attributes are found in the documentation.

## Styling the Horizontal Rule

To replicate the thicker horizontal rule found in certain web designs, you can specify the `size` attribute. For example:

```html
<hr size="3" noshade>
```

This code creates a horizontal rule with a height of three pixels and no shading, resembling the style of the referenced webpage.