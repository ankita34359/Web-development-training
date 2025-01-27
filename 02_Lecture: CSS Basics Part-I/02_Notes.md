# CSS Basics Part-I

In this lecture, I learned the foundational concepts of CSS (Cascading Style Sheets). CSS is used to style and enhance the appearance of HTML elements, making web pages visually appealing and user-friendly. This lecture introduced various CSS properties and techniques, applied across pages like Home, About, and Contact.

---

## Key Concepts Learned

### CSS Basics

#### Ways to Add CSS

- **Inline CSS:** Using the style attribute within an HTML element.

   ```html
      <h1 style="color: blue;">Hello, World!</h1>
   ```

- **Internal CSS:** Using a <style> tag within the <head> section of the HTML file.

   ```html
    <style>
    h1 {
    color: blue;
    }
    </style>
  ```

- **External CSS:** Linking an external .css file using the <link> tag.

  ```html
   <link rel="stylesheet" href="styles.css">
  ```

---

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

---

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

---

#### 3.)Box Modeling Properties: 

##### a.) Padding

The table below provides a summary of CSS padding properties, their options, and values:


| **Property**       | **Options/Values**                       |
|---------------------|------------------------------------------|
| **padding**        | `auto`, unit values (`px`, `%`, `em`)    |
| **padding-top**    | Specific padding for the top             |
| **padding-right**  | Specific padding for the right           |
| **padding-bottom** | Specific padding for the bottom          |
| **padding-left**   | Specific padding for the left            |


The tables below summarize the options and values for CSS Margin and Border properties:

##### b.) Margin Properties

The tables below summarize the options and values for CSS Margin properties:


| **Property**       | **Options/Values**                       |
|---------------------|------------------------------------------|
| **margin**         | `auto`, unit values (`px`, `%`, `em`)    |
| **margin-top**     | Specific margin for the top              |
| **margin-right**   | Specific margin for the right            |
| **margin-bottom**  | Specific margin for the bottom           |
| **margin-left**    | Specific margin for the left             |


##### c.)  Border Properties

The tables below summarize the options and values for CSS Border properties:


| **Property**       | **Options/Values**                                                                 |
|---------------------|------------------------------------------------------------------------------------|
| **border**         | `border-width border-style border-color` (e.g., `1px solid black`)                 |
| **border-width**   | `thin`, `medium`, `thick`, unit values (`px`)                                      |
| **border-style**   | `none`, `solid`, `dashed`, `dotted`, `double`, `groove`, `ridge`, `inset`, `outset`, `hidden` |
| **border-color**   | Any valid color                                                                    |
| **border-radius**  | Numeric values (e.g., `10px`, `50%` for circular corners)                          |

---

#### 4.) Display and Positioning Properties

The table below summarizes the options and values for CSS display and positioning properties:

| **Property**         | **Options/Values**                                                                           |
|-----------------------|----------------------------------------------------------------------------------------------|
| **display**          | `block`, `inline`, `inline-block`, `flex`, `grid`, `none`, `inline-flex`, `table`, `table-cell`|
| **position**         | `static`, `relative`, `absolute`, `fixed`, `sticky`                                          |
| **z-index**          | Numeric value (e.g., `1`, `1000`)                                                            |
| **top, right, bottom, left** | Unit values (`px`, `%`)                                                              |
| **overflow**         | `visible`, `hidden`, `scroll`, `auto`                                                        |

---

#### 5.) Flexbox Properties

The table below summarizes the options and values for CSS Flexbox properties:

| **Property**         | **Options/Values**                                                                           |
|-----------------------|----------------------------------------------------------------------------------------------|
| **flex-direction**   | `row`, `row-reverse`, `column`, `column-reverse`                                              |
| **justify-content**  | `flex-start`, `flex-end`, `center`, `space-between`, `space-around`, `space-evenly`           |
| **align-items**      | `flex-start`, `flex-end`, `center`, `stretch`, `baseline`                                     |
| **flex-wrap**        | `nowrap`, `wrap`, `wrap-reverse`                                                             |
| **flex-grow**        | Numeric value (`0`, `1`, etc.)                                                               |
| **flex-shrink**      | Numeric value                                                                                |
| **align-content**    | `flex-start`, `flex-end`, `center`, `space-between`, `space-around`, `stretch`               |

---

#### 6.) Pseudo-classes

The table below summarizes common CSS pseudo-classes, their usage, and when they apply:


| **Pseudo-Class**    | **Usage**                                                        |
|----------------------|------------------------------------------------------------------|
| `:hover`            | Applies styles when the mouse is over an element                |
| `:focus`            | Applies styles when an element (e.g., input) is focused         |
| `:active`           | Applies styles when an element is being clicked                 |
| `:first-child`      | Applies styles to the first child of an element                 |
| `:last-child`       | Applies styles to the last child of an element                  |
| `:nth-child(n)`     | Applies styles to the nth child of an element                   |

---

##  Practical Applications

### Home Page

- Applied a background-color for the body.
- Styled the navigation bar using display: flex and added hover effects to links.
- Used font-family and font-size for headings and paragraphs.

### About Page

- Created a flexbox layout for presenting information side-by-side.
- Used padding, margin, and border to create spacing and separation.

### Contact Page

- Styled the form inputs with padding and border-radius.
- Added a hover effect to the submit button.
- Used cursor: pointer for buttons and links.

---

## Conclusion

This lecture provided a comprehensive understanding of CSS properties and their applications. By combining these properties, I can create visually appealing and responsive web pages.
