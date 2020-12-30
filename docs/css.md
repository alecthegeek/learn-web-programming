# Cascading style sheets (CSS)

Styles can be defined in three locations

1. Embedded in the html element with the `style` attribute. **Don't do this**
2. In the HTML head inside the `<style>` element
3. In a separate file referenced by the `<link>` element (e.g. `<link rel="stylesheet" type="text/css" href="css/style.css">`). This is the preferred approach so that styles are defined in one place and can be used across multiple html files

## CSS format

```
selector{ property: value ; property : value; .... }
```

Selector:

1. An element name e.g. h1 would apply the style to all `h1` elements
2. Class, the format is `.class {...}` (notice dot)
3. ID


Colour values can be names, html5 names, hex, or RGB triplets (`rgb(0,0,255)`)


[![CSS Crash Course For Absolute Beginners](https://img.youtube.com/vi/yfoY53QXEnI/0.jpg)](https://www.youtube.com/watch?v=yfoY53QXEnICSS)

([files](https://www.traversymedia.com/downloads/csscrashcourse.zip) for the above)

[![10 modern layouts in 1 line of CSS](https://img.youtube.com/vi/qm0IfG1GyZU/0.jpg)](https://www.youtube.com/watch?v=qm0IfG1GyZU)
