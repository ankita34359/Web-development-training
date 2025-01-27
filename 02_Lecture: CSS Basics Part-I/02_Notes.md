# CSS Basics Part-I

In this lecture, I learned the foundational concepts of CSS (Cascading Style Sheets). CSS is used to style and enhance the appearance of HTML elements, making web pages visually appealing and user-friendly. This lecture introduced various CSS properties and techniques, applied across pages like Home, About, and Contact.

## Key Concepts Learned

### CSS Basics

#### Ways to Add CSS

- **Inline CSS:** Using the style attribute within an HTML element.

   ```html
      <h1 style="color: blue;">Hello, World!</h1>
   ```

**Internal CSS:** Using a <style> tag within the <head> section of the HTML file.

```html
<style>
    h1 {
        color: blue;
    }
</style>
```

**External CSS:** Linking an external .css file using the <link> tag.

```html
<link rel="stylesheet" href="styles.css">
```

### Core CSS Properties

#### 1.) Background Properties

The table below provides a summary of common CSS background properties, their options, and values:

| **Property**           | **Options/Values**                                                                                       |
|-------------------------|---------------------------------------------------------------------------------------------------------|
| **background-color**    | Any valid color (e.g., `red`, `#FF5733`, `rgb(255,87,51)`)                                              |
| **background-image**    | `url("image.jpg")`, `none`, `linear-gradient()`, `radial-gradient()`                                    |
| **background-repeat**   | `repeat`, `repeat-x`, `repeat-y`, `no-repeat`, `space`, `round`                                         |
| **background-position** | `top`, `center`, `bottom`, `left`, `right`, `x% y%`, `xpx ypx`                                          |
| **background-size**     | `auto`, `cover`, `contain`, `x%`, `xpx`                                                                 |
| **background-attachment**| `scroll`, `fixed`, `local`                                                                             |
| **background-clip**     | `border-box`, `padding-box`, `content-box`                                                              |
| **background-origin**   | `border-box`, `padding-box`, `content-box`                                                              |

#### 2.) Text Properties

The table below provides a summary of common CSS text properties, their options, and values:

| **Property**         | **Options/Values**                                                                                     |
|-----------------------|-------------------------------------------------------------------------------------------------------|
| **color**            | Any valid color                                                                                      |
| **font-family**      | `Arial`, `Verdana`, `sans-serif`, etc. (comma-separated values for fallbacks)                         |
| **font-size**        | `xx-small`, `x-small`, `small`, `medium`, `large`, `x-large`, `xx-large`, `%`, `px`, `em`, `rem`      |
| **font-style**       | `normal`, `italic`, `oblique`                                                                         |
| **font-weight**      | `normal`, `bold`, `bolder`, `lighter`, numeric values (`100` to `900`)                                |
| **line-height**      | `normal`, numeric value (`1.5`), unit values (`20px`, `150%`)                                         |
| **text-align**       | `left`, `right`, `center`, `justify`, `start`, `end`                                                 |
| **text-decoration**  | `none`, `underline`, `overline`, `line-through`, `blink` (rarely used)                                |
| **text-transform**   | `capitalize`, `uppercase`, `lowercase`, `none`                                                       |
| **letter-spacing**   | `normal`, unit value (`2px`)                                                                          |
| **word-spacing**     | `normal`, unit value (`4px`)                                                                          |
