# "Advanced" HTML

"Advanced" means stuff Alec is not familiar with.

Note: A lot of this material is adapted from [w3schools.com](https://www.w3schools.com/)

## `class` attribute

The class attribute specifies one **or more** class names for an element.

The class attribute is predominantly used to point to a class in a style sheet. However, it can also be used by a JavaScript (via the HTML DOM) to make changes to HTML elements with a specified class. However class names can be used multiple times, so generally it's more useful to use the attribute `id` to access DOM elements frm js.

All HTML elements can be given a class attribute

The value of `class` specifies one or more class names for an element. To specify multiple classes, separate the class names with a space, e.g. `<span class="left important">`. This allows you to combine several CSS classes for one HTML element.

Naming rules: Must begin with a letter A-Z or a-z
Can be followed by: letters (A-Za-z), digits (0-9), hyphens ("-"), and underscores ("_")

## `id` attribute

The id attribute specifies a unique id for an HTML element (the value must be unique within the HTML document).

All HTML elements can be given an id attribute.

Example `<h1 id="myHeader">Hello World!</h1>`

The id attribute is most used: by JavaScript (via the HTML DOM) to manipulate the element with the specific id; as the target of an href; and to point to a style in a style sheet. In the last two cases prefix the id with `#`.

## `onclick` attribute

Execute the specified JS code when the element received a mouse click

Example:

Click on a `<button>` element to display the current day, date and time:

```html
<button id="demo" onclick="getElementById('demo').innerHTML = Date()">What is the time?</button>
```

Supported HTML tags: All HTML elements, **EXCEPT**: `<base>`, `<bdo>`, `<br>`, `<head>`, `<html>`, `<iframe>`, `<meta>`, `<param>`, `<script>`, `<style>`, and `<title>`.

See also Javascript `object.onclick = function(){myScript};` (where `object` is something in the DOM)

More info [here](https://www.w3schools.com/jsref/event_onclick.asp)

## forms

An HTML form is used to collect user input. The user input is most often sent to a server for processing or processed via js

The `<form>` element is a container for different types of input elements, such as: text fields, checkboxes, radio buttons, submit buttons, etc

### `label` element

Used for [protected fields](https://link.springer.com/referenceworkentry/10.1007%2F1-4020-0613-6_14968https://link.springer.com/referenceworkentry/10.1007%2F1-4020-0613-6_14968)

### `input` element

[Unprotected field](https://link.springer.com/referenceworkentry/10.1007%2F1-4020-0613-6_20494). An input element has a type. Always specify the type

| Type                           | Notes                      |
|--------------------------------|----------------------------|
|`<input type="button">`         |                            |
|`<input type="checkbox">`       |                            |
|`<input type="color">`          |                            |
|`<input type="date">`           |                            |
|`<input type="datetime-local">` |                            |
|`<input type="email">`          |                            |
|`<input type="file">`           |                            |
|`<input type="hidden">`         |                            |
|`<input type="image">`          |                            |
|`<input type="month">`          |                            |
|`<input type="number">`         |                            |
|`<input type="password">`       |                            |
|`<input type="radio">`          |                            |
|`<input type="range">`          |                            |
|`<input type="reset">`          |                            |
|`<input type="search">`         |                            |
|`<input type="submit">`         |                            |
|`<input type="tel">`            |                            |
|`<input type="text">`           |  Default                   |
|`<input type="time">`           |                            |
|`<input type="url">`            |                            |
|`<input type="week">`           |                            |


## button element

The `<button>` tag defines a clickable button. This can be located inside a form or standalone.

You can style a button

**Always** give a button a type

You can use the `onclick` attribute
