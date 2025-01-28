# CSS Basics Part III

## Lecture Overview

In this lecture, we explored advanced CSS properties like transform, transition, and animation. These properties allow us to create interactive and visually dynamic effects, enhancing user experience on your website.

This document explains these properties in detail with practical examples to help you understand how to use them effectively.

---

## 1. Transform Property

The transform property allows you to modify the shape, size, and position of elements without affecting the document flow. It supports various transformation functions such as translation, rotation, scaling, and skewing.

```css
transform: function(value);
```

## Functions and Examples

translate(x, y)
Moves an element from its current position by the specified x (horizontal) and y (vertical) values.

```css
div {
    transform: translate(50px, 20px);
}
```
