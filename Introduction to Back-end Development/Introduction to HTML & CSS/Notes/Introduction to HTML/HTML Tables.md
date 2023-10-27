# Structured Tables in HTML

Tables are a powerful way to organize and display data on web pages. We'll learn how to create tables to represent information like work experience, and we'll discuss the basic structure of HTML tables.

## Understanding HTML Tables

HTML tables are used to organize and present data in a tabular form. They consist of rows and columns, where each cell can contain data. Tables provide an organized layout, making it easier to display various types of information neatly.

## Creating a Basic Table

To create a basic table in HTML, follow this structure:

```html
<table>
  <tr>
    <th>Column 1</th>
    <th>Column 2</th>
  </tr>
  <tr>
    <td>Data 1</td>
    <td>Data 2</td>
  </tr>
</table>
```

- `<table>`: The table container.
- `<tr>`: Table rows.
- `<th>`: Table header cells (for column headings).
- `<td>`: Table data cells (for data).

Each row (`<tr>`) contains cells (`<th>` for headers or `<td>` for data). You can create more rows and cells as needed.

## Adding Table Headers

To make your table more structured, use table headers for column headings. Headers are created using the `<th>` element inside the first row (`<tr>`) of the table:

```html
<table>
  <tr>
    <th>Date</th>
    <th>Work</th>
  </tr>
  <tr>
    <td>2010-2013</td>
    <td>Lead Developer at Tempo App</td>
  </tr>
  <tr>
    <td>2010</td>
    <td>Researcher at Institute of Cognitive Neurosciences</td>
  </tr>
</table>
```

Headers are typically rendered in bold by default, making them stand out from regular data cells.

## Styling Tables

HTML tables have limited styling options using HTML attributes, but these are considered deprecated. It's essential to separate structure (HTML), presentation (CSS), and behavior (JavaScript) in web development.

We can use CSS to style tables, such as adding borders, background colors, padding, and more. However, detailed styling is typically done using CSS, which we'll cover in future lessons.

## Recap

- Tables are used to organize and display structured data.
- HTML tables consist of rows (`<tr>`) and cells (`<th>` for headers or `<td>` for data).
- Tables can have headers to label columns.
- Tables are primarily for structure; styling is done using CSS.