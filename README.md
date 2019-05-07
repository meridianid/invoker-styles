![alt text][cover]
[![alt text][mission]](http://meridian.id)

# Invoker Styles

1. [Overview](#overview)
    * [What it is](#what-it-is)
    * [What is is NOT](#what-it-is-not)
2. [Getting Started](#getting-started)
3. [Principles](#principles)
    * [A11y First](#a11y-first)
    * [Gestalt](#gestlat)
4. [Colors](#colors)
    * [Brands](#brand)
    * [Darks](#darks)
    * [Light](#light)
    * [Tone](#tone)
    * [Backgrounds](#backgrounds)
5. [Spaces](#spaces)
    * [Steps](#steps)
    * [Inset](#inset)
    * [Stack](#Stack)
    * [Vertical](#vertical)
    * [Horizontal](#horizontal)
    * [Inline](#inline)
6. [Typography](#typography)
    * [Display](#display)
    * [Heading](#heading)
    * [Body](#body)
    * [Caption](#caption)
7. [Style Tokens](#style-tokens)

## Overview

A styling language for a better collaboration between designer and developer.

### What it is

It is just a spec. And for now, we are only going to provide the Sass (using SCSS) implementation and also the android implementation is coming soon.

### What it is not

It is not a CSS framework, UI library, or any kind of framework

---

## Getting Started

How to make use of this styling language?

---

## Principles

### A11y First

### Gestalt

---

## Colors

### Brands

### Darks

### Light

### Tone

### Backgrounds

---

## Spaces

Spacing tokens are used for padding, margins, and position coordinates. Each value of spaces are counted based on **16px**.

### Steps

![alt text][space-steps]

### Inset

A spacing area on all four sides of the box.

![alt text][space-inset]

### Stack

Add spacing area at the bottom side of the box.

![alt text][space-stack]

### Vertical

Extending the stack concept, vertical adds spaces at the top and bottom side of the box.

### Inline

Add spacing area at the right side of the box.

![alt text][space-inline]

### Horizontal

Expanding the inline concept, horizontal adds spaces at the left and right side of the box.

---

## Typography

> Text is one of the main way we can deliver the information to the user. Keeping consist and sticking to logical hierarchies ensures that elements in the UI are clear and easily recognizable when scanning the page.

In our works, we encountered so many type-scale variations. And each of our works, sometimes, has it's own specific requirements regarding the typography.

We learned that having our own shared language and consistent in every project to communicate type-scale and it's properties would really improving our workflow. So, to communicate the typography better in our team, we give each type-scale it's own name. That way, each team member doesn't need to pay attention to what're the properties of each type scale and it's implementaiton details. All they should care about is the name and communicate them using it's name.

And to avoid confusion and the burden of having to memorize every names whenever we start new project, we are using the generic and low-level terms instead of a too high-level and specific name like **title, subtitle, overline, etc.**

### Display

A really big texts. It's purpose is to attract users attention (i.e a tagline). It's mostly used in a marketing site (i.e. landing page, company profile, event website, etc), and rarely used in mobile app or an internal web app because it will take a huge amount of space.

* **display1** (128/128 - 800)
* **display2** (96/96 - 800)
* **display3** (64/64 - 800)

### Heading

Heading texts used to emphasize the structure of your interfaces. The combination between it's sizes and weights makes your content distinct from each other, hence, helping users when they skim and read them.

* **heading1** (46/52 - 700)
* **heading2** (32/36 - 700)
* **heading3** (24/30 - 700)
* **heading3Alt** (24/30 - 500)
* **heading4** (18/26 - 700)
* **heading4Alt** (18/26 - 500)
* **heading5** (16/22 - 500)
* **heading5Alt** (16/22 - 700)
* **heading6** (14/18 - 500)
* **heading6Alt** (14/18 - 700)

### Body

Body texts primarily used for paragraphs.

* **bodyLarge** (18/26 - 400)
* **bodyMedium** (16/22 - 400)
* **bodySmall** (14/18 - 400)

### Caption

Caption texts are mainly used for caption, helper, hints, etc. Because of it's size, be sure to make your caption's color comply to a11y requirements.

* **captionSmall** (11/12 - 400)
* **captionSmallAlt** (11/12 - 500)
* **captionLarge** (12/16 - 400)
* **captionLargeAlt** (12/16 - 500)

---

## Style Tokens

[cover]: https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/cover-alt.png "Invoker Styles"
[mission]: https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/mission.png "Invoker Styles"

<!-- SPACES -->
[space-steps]: https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/space-steps.png "Space Steps"
[space-inset]: https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/space-inset.png "Space Inset"
[space-stack]: https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/space-stack.png "Space Stack"
[space-inline]: https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/space-inline.png "Space Inline"
