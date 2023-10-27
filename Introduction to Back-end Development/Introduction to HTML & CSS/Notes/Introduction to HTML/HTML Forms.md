# HTML Forms

Forms are essential for user interaction on websites, and even though their full functionality requires JavaScript (which we'll cover later), we can explore how to structure them in HTML.

## Basic Form Elements

### Input Elements

To create a basic form, you'll use the `<form>` element. Within a form, you typically include various input elements where users can provide data.

#### Text Input

For capturing text data, you can use the `<input>` element with the `type` attribute set to "text." This provides a simple text box where users can enter information. For example:

```html
<label>Your Name: <input type="text"></label>
```

#### Submit Button

To submit the form, you can use another `<input>` element with the `type` attribute set to "submit." This creates a submit button:

```html
<input type="submit">
```

#### Checkbox Input

For yes/no questions or multiple choices, you can use checkboxes. Here's an example:

```html
<label>
  <input type="checkbox" name="subscribe"> Subscribe to our newsletter
</label>
```

#### Password Input

When capturing sensitive data like passwords, you can use the `<input>` element with the `type` attribute set to "password." The entered text is typically masked:

```html
<label>Password: <input type="password"></label>
```

#### Color Input

You can even have users select a color using the color input type:

```html
<label>Choose a color: <input type="color"></label>
```

### Try Different Input Types

Explore various input types like date pickers, radio buttons, and more. Create an HTML file and use these input types to see how they work interactively.