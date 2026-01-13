# Short Response Questions

Answer the following questions in your own words. Each response should be 2-4 sentences.

## Question 1: HTML Structure

What is the difference between the `<head>` and `<body>` sections of an HTML document? What kind of content goes in each?

**Your Answer:**

## Question 2: Semantic HTML

Why should we use semantic elements like `<header>`, `<main>`, and `<footer>` instead of using `<div>` tags for everything?

**Your Answer:**

Semantic HTML elements like <header>, <main>, and <footer> give meaning to the structure of a webpage, while <div> elements do not. These semantic tags help screen readers and other assistive technologies understand and navigate content more easily. They also improve search engine optimization by clearly identifying important sections of a page. Using semantic elements makes HTML more readable and maintainable for developers. <div> tags should be used only when no semantic element accurately describes the content.

## Question 3: CSS Selectors

Given the following HTML:

```html
<ul>
  <li class="vegetable">Carrots</li>
  <li class="vegetable">Broccoli</li>
  <li class="fruit" id="favorite">Mango</li>
</ul>
```

Write THREE different CSS rules:

1. One that makes ALL list items have a `yellow` background
2. One that makes only the vegetables have `green` text color
3. One that makes only the Mango `bold`

**Your Answer:**

```css
ul > li {
  background-color: yellow;
}
ul > .vegetable {
  color: green;
}
ul > #favorite {
  font-weight: bold;
}
```

## Question 4: The Box Model

In your own words, explain the four parts of the CSS box model (content, padding, border, margin). What is the purpose of each part?

**Your Answer:**
The CSS box model is a concept where every HTML element is treated as a rectangular box. The content is the innermost part of the box and contains the actual text, image, or element itself. Padding surrounds the content and controls the space between the content and the border. The border wraps around the padding and defines the visible edge of the element, with properties such as width, style, and color. The margin is the outermost layer and controls the space between the element and other elements on the page.

## Question 5: Box-Sizing

What problem does `box-sizing: border-box` solve? Why do we include it in a CSS reset at the top of our CSS files?

**Your Answer:**

box-sizing: border-box solves the problem of elements unexpectedly growing in size when padding or borders are added. By default, padding and borders are added on top of an element’s width and height, which can break layouts. With border-box, the padding and border are included inside the defined width and height, making sizing more predictable.
We include it in a CSS reset at the top of our CSS files to ensure consistent and predictable layout behavior across all elements. This prevents layout bugs, reduces the need for recalculations, and makes designing responsive layouts much easier from the start.

## Question 6: Display Property

What is the difference between `display: block`, `display: inline`, and `display: inline-block`? Give an example of when you might use `inline-block`.

**Your Answer:**

The default display of most HTML elements is display: block, which allows the content to take up 100% of the page and allows you to define the width and height of the content. Display: inline when applied to an element allows it to take up as much space as the content, and if there is enough space, other elements can go on the same line. However, it does not allow you to define a width or height. Display: inline-block allows you to have the best of both worlds, which is the ability to control width and height, and also allows other elements to go on the same line if there is enough space for it to fit. You might use inline-block when you have an element that is taking up 100% of the width, and you want to have an element below it go on the same line, but also control the width of that element.
