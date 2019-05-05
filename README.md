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
    * [Inset](#inset)
    * [Inline](#inline)
    * [Stack](#Stack)
    * [Squish](#squish)
    * [Stretch](#stretch)
    * [Vertical](#vertical)
    * [Horizontal](#horizontal)
6. [Typography](#typography)
    * [Display](#display)
    * [Heading](#heading)
    * [Body](#body)
    * [Caption](#caption)
7. [Style Tokens](#style-tokens)

## Overview

A styling language for a better collaboration between designer and developer.

---

### What it is

It is just a spec, and we are only going to provide the Sass (with SCSS) implementation and the android implementation is coming soon.

---

### What it is not

It is not a UI library or framework

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

### Inset

### Inline

### Stack

### Squish

### Stretch

### Vertical

### Horizontal

---

## Typography

In our works, we encountered so many type-scale variations. And each of our works, sometimes, has it's own specific requirements regarding the typography.

We learned that having our own shared language and consistent in every project to communicate type-scale and it's properties would really improving our workflow. So, to communicate the typography better in our team, we give each type-scale it's own name. That way, each team member doesn't need to pay attention to what're the properties of each type scale and it's implementaiton details. All they should care about is the name and communicate them using it's name.

And to avoid confusion and the burden of having to memorize every names whenever we start new project, we are using the generic and low-level terms instead of a too high-level and specific name like **title, subtitle, overline, etc.**

### Display

A really big texts. It's purpose is to attract users attention (i.e a tagline). It's mostly used in a marketing site (i.e. landing page, company profile, event website, etc), and rarely used in mobile app or an internal web app because it will take a huge amount of space.

* **display1**
* **display2**
* **display3**

### Heading

Heading texts used to emphasize the structure of your interfaces. The combination between it's sizes and weights makes your content distinct from each other, hence, helping users when they skim and read them.

* **heading1**
* **heading2**
* **heading3**
* **heading3Alt**
* **heading4**
* **heading4Alt**
* **heading5**
* **heading5Alt**
* **heading6**
* **heading6Alt**

### Body

Body texts primarily used for paragraphs.

* **bodyLarge**
* **bodyMedium**
* **bodySmall**

### Caption

Caption texts are mainly used for caption, helper, hints, etc. Because of it's size, be sure to make your caption texts compatible to a11y requirements.

* **captionSmall**
* **captionSmallAlt**
* **captionLarge**
* **captionLargeAlt**

---

## Style Tokens

[cover]: https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/cover-alt.png "Invoker Styles"
[mission]: https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/mission.png "Invoker Styles"