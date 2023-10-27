# HTML Image Elements

Let's explore how to add images to your website using the HTML `img` element. The `img` element is a self-closing tag, meaning it doesn't need a closing tag.

To display an image on your website, you must specify the image source, which can be either a URL (for images hosted online) or a local image in the same directory as your website files.

## Adding an Image from the Web

Let's begin by adding an image from the web. You can find an image online, right-click on it, and copy the image address (URL). For example, you could use your own Twitter or Facebook profile picture.

Next, insert the image into your website using the `img` tag. You need to provide the `src` (source) attribute with the URL and an optional `alt` (alternative text) attribute, which describes the image for accessibility and search engine optimization.

Here's an example:

```html
<img src="https://example.com/your-image.jpg" alt="Description of your image">
```

The `alt` text is important for SEO and accessibility, as it helps search engines understand your content and assists users with disabilities.

## Adding a Local Image

To include a local image (an image stored on your computer) in your website, first, ensure that the image is located in the same directory as your HTML file. You can then reference it using the `src` attribute without a URL.

For example, if your image is named "my-image.jpg," you can use this code:

```html
<img src="my-image.jpg" alt="Description of your local image">
```

Remember to provide a meaningful `alt` text for accessibility and SEO purposes.

## Displaying the Image

Once you've added the image element with the correct `src` and `alt` attributes, save your HTML file and refresh your webpage to see the image displayed.
