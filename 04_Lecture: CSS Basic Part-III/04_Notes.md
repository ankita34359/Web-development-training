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

1.) translate(x, y)

Moves an element from its current position by the specified x (horizontal) and y (vertical) values.

```css
div {
    transform: translate(50px, 20px);
}
```

2.) scale(x, y)

Scales an element's size horizontally (x) and vertically (y).

```css
div {
    transform: scale(1.5, 1.5); /* Enlarges element by 1.5 times */
}
```

3.) rotate(angle)

Rotates an element by the specified angle (in degrees).

```css
div {
    transform: rotate(45deg);
}
```

4.) skew(x-angle, y-angle)

Skews an element along the x and y axes.

```css
div {
    transform: skew(20deg, 10deg);
}
```

5.) matrix(a, b, c, d, e, f)

Applies a combination of transformations using a transformation matrix.

```css
div {
    transform: matrix(1, 0, 0, 1, 50, 50); /* Combines translate and scale */
}
```

## 2. Transition Property

The transition property adds smooth changes between property values over a specified duration. It is often used for hover effects and animations.

```css
transition: property duration timing-function delay;
```

### Parameters

- **property:** The CSS property to be transitioned (e.g., background-color, transform).
- **duration:** The time (e.g., 2s, 500ms) the transition takes.
- **timing-function:** Defines the speed curve (ease, linear, ease-in, ease-out, etc.).
- **delay:** The wait time before the transition starts (optional).

#### Example: 

```css
  button {
    background-color: blue;
    transition: background-color 0.5s ease-in-out;
}

button:hover {
    background-color: green;
}
```

## 3. Animation Property

The animation property enables the creation of keyframe-based animations. You can control the timing, duration, and other parameters of an animation.

### Keyframes

Keyframes define the stages of an animation by specifying styles at various points.

```css
@keyframes animation-name {
    from {
        property: value;
    }
    to {
        property: value;
    }
}
```

Syntax: 

```css
animation: name duration timing-function delay iteration-count direction;
```

#### Parameters

- **name:** The name of the keyframes.
- **duration:** Duration of the animation (e.g., 2s).
- **timing-function:** Defines the speed curve.
- **delay:** Wait time before animation starts.
- **iteration-count:** Number of times the animation runs (infinite for continuous looping).
- **direction:** Direction of the animation (normal, reverse, alternate, etc.).

#### Example: 

```css
@keyframes slide {
    from {
        transform: translateX(0);
    }
    to {
        transform: translateX(100px);
    }
}

div {
    animation: slide 2s ease-in-out infinite;
}
```

## Combining Transform, Transition, and Animation

You can combine these properties to create dynamic effects.

#### Example:

```css
<div class="animated-box"></div>
```

```css
.animated-box {
    width: 100px;
    height: 100px;
    background-color: red;
    transform: scale(1);
    transition: transform 0.5s ease-in-out, background-color 0.5s;

    animation: color-change 3s linear infinite;
}

.animated-box:hover {
    transform: scale(1.2);
    background-color: blue;
}

@keyframes color-change {
    0% {
        background-color: red;
    }
    50% {
        background-color: yellow;
    }
    100% {
        background-color: red;
    }
}
```

### Effect

- When hovered, the box scales up and changes color.
- The color also cycles through red and yellow in a continuous animation.
