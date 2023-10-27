# Structuring Your Website Layout Using HTML Tables

One common layout you might want to create is similar to Thomas Cormen's website, where you have an image on the left and accompanying content (name, title, blurb) on the right. We'll use HTML tables to achieve this layout since we haven't covered CSS and styling yet.

## Creating a Side-by-Side Layout

To create a side-by-side layout with an image on the left and content on the right, we'll use an HTML table. Here's how we can do it:

```html
<table>
  <tr>
    <td><!-- Image goes here --></td>
    <td><!-- Content goes here --></td>
  </tr>
</table>
```

- `<table>`: The table container.
- `<tr>`: Table rows.
- `<td>`: Table data cells (for holding content).

The first `<td>` element will contain the image, and the second `<td>` element will hold all the content. 

## Styling the Layout

As we haven't covered CSS and styling yet, you can control the space between the image and content using the `cellspacing` attribute within the `<table>` element. For example, if you want to increase the space between cells, you can set `cellspacing` like this:

```html
<table cellspacing="20">
  <tr>
    <td><!-- Image goes here --></td>
    <td><!-- Content goes here --></td>
  </tr>
</table>
```

In this example, the `cellspacing` is set to 20 pixels, creating some spacing between the image and content cells. Adjust this value to achieve your desired spacing.

Remember that this is a basic way to create a layout with HTML tables, and more advanced styling and layout techniques are typically handled with CSS, which we'll cover in future lessons.

With these techniques, you can structure your website layout even without CSS knowledge. In our next lessons, we'll delve deeper into CSS to enhance the styling and appearance of your website.
