# CSS Basics Part II

## Lecture Overview

In this lecture, I learned about CSS properties related to Positioning and Backgrounds. These properties are fundamental in creating visually appealing layouts and controlling the placement of elements on a webpage.

This document provides a detailed explanation of the properties covered in the lecture, with examples to help us understand how to use them effectively.

## Position Properties

CSS `position` defines how an element is positioned in the document flow. There are five main values: `static`, `relative`, `absolute`, `fixed`, and `sticky`. Here's an overview of each:

### 1. position: static (Default)

- **Description:** The default positioning of elements. Elements are placed in the natural flow of the document.
- **Use Case:** No additional positioning; the browser determines the position.

```css
div {
    position: static;
}
```

### 2. position: relative

- **Description:** Positions the element relative to its normal position. You can use top, right, bottom, or left to move it.
- **Use Case:** Useful for slight adjustments or creating offset effects.

```css
  div {
    position: relative;
    top: 10px;
    left: 20px;
}
```

### 3. position: absolute

- **Description:** Removes the element from the document flow and positions it relative to its nearest positioned ancestor (not static).
- **Use Case:** Commonly used for modals, dropdown menus, or overlays.

```css
  div {
    position: absolute;
    top: 50px;
    left: 30px;
}
```

### 4. position: fixed

- **Description:** Positions the element relative to the viewport. The element stays fixed in place when scrolling.
- **Use Case:** Perfect for sticky headers, footers, or side navigation bars.
