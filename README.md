# Frontend Mentor - Recipe page solution

This is a solution to the [Recipe page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### Screenshot

![](./screenshot.jpg)

Add a screenshot of your solution. The easiest way to do this is to use Firefox to view your project, right-click the page and select "Take a Screenshot". You can choose either a full-height screenshot or a cropped one based on how long the page is. If it's very long, it might be best to crop it.

Alternatively, you can use a tool like [FireShot](https://getfireshot.com/) to take the screenshot. FireShot has a free option, so you don't need to purchase it. 

Then crop/optimize/edit your image however you like, add it to your project, and update the file path in the image above.

**Note: Delete this note and the paragraphs above when you add your screenshot. If you prefer not to add a screenshot, feel free to remove this entire section.**

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- [React](https://reactjs.org/) - JS library
- [Next.js](https://nextjs.org/) - React framework
- [Styled Components](https://styled-components.com/) - For styles

**Note: These are just examples. Delete this note and replace the list above with your own choices**

### What I learned

## `<article>` vs `<section>`

### 🧾 Quick Comparison Table

| Element | Meaning | Use case | Rule |
|--------|--------|----------|------|
| `<article>` | Complete, independent content | Recipe, blog, product | Can stand alone |
| `<section>` | Themed part of content | Ingredients, steps | Must have a heading (**IMPORTANT**) |

---

### 🧠 Mental Rules (Easy Revision)

- If it can be shared alone → `<article>`
- If it’s a part of something → `<section>`

---

### ❓ What does “themed part of content” mean?

A **themed part of content** is a group of related information that:
- Focuses on **one topic**
- Can be described by a **single heading**

---

### 🤔 Think in human terms 🧠

Imagine explaining your recipe to someone:

> “First I’ll tell you **ingredients**.  
> Then I’ll explain **instructions**.  
> After that, **nutrition**.”

Each of those is a **theme**.


---

## 🎨 How to Make List Dots (Bullets) Colored in CSS

There are **two ways** to change the color of list dots (`ul > li`) in CSS.

### ✅ Method 1: Using `::marker`

The modern and simplest approach.

```css
ul li::marker {
  color: red;
  font-size: 18px; /* optional */
}


### ✅ Method 2: Using `Use list-style: none and create your own dot.`

```css
ul {
  list-style: none;
}

ul li {
  position: relative;
  padding-left: 20px;
}

ul li::before {
  content: "•";
  color: green;
  font-size: 20px;
  position: absolute;
  left: 0;
}

---

## Logical Margins (Inline)

- `margin-inline-start` and `margin-inline-end` define horizontal margins based on the **text direction**, not physical left/right.
- In **LTR** layouts:  
  - `inline-start` → left  
  - `inline-end` → right
- In **RTL** layouts, they automatically flip.

**Shorthand**
- `margin-inline: value;` → applies to both start and end
- `margin-inline: start end;` → sets start and end separately

These logical properties are recommended for **responsive and multilingual layouts**.



## Mistake I did

- I always think in css for common css property I will create, common class.
- But What I think I should create class for element if same element used at another place just reuse it (Make Simple)
- Always provide consitent class name 
### Useful resources

- [Responsive Image Resizing](https://www.youtube.com/watch?v=gn0OaxS1OdY) - This is an amazing article which helped me finally understand XYZ. I'd recommend it to anyone still learning this concept.
- [Responsive Image Resizing More optimized](https://www.youtube.com/watch?v=345V2MU3E_w) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.
- [KV A practical guide to responsive web design] (https://www.youtube.com/watch?v=x4u1yp3Msao)


## Author
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/@apsbundela)
