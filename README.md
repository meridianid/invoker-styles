![alt text][cover]
[![alt text][mission]](http://meridian.id)

# Invoker Styles

1. [Overview](#overview)
    * [What it is](#what-it-is)
    * [What is is NOT](#what-it-is-not)
2. [Getting Started](#getting-started)
3. [Principles](#principles)
    * [A11y First](#a11y-first)
    * [Gestalt](#gestalt)
4. [Colors](#colors)
    * [Brands](#brands)
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

## Overview

A styling language for a better collaboration between designer and developer.

### What it is

It is just a spec. And for now, we are only going to provide the Sass (using SCSS) implementation and also the android implementation is coming soon.

### What it is not

It is not a CSS framework, UI library, or any kind of framework

---

## Getting Started

Because of the nature of consultancy works, we can't use a single brand for all of our clients. Hence, for now, the only way to use the implementation of SCSS without doing too many overwrites is by manually copying the whole modules folder and change all the tokens values according to the project brand.

If you are using relative path, add an entry point like `tokens.scss`  in your `src` would make it easier for you to import the files within your styles. Because you would likely to import the style tokens for each of your styles. But if you are using the invoker starters, need not to worry, the setup is already done for you.

But if you just tinkering around and want to use the brand of Meridian.id in your project, you can add the modules as packages to your project through npm.

```shell
npm install --save invoker-base invoker-layout invoker-tokens
```

or if you are using `yarn`

```shell
yarn add invoker-base invoker-layout invoker-tokens
```

Then, you can just import the modules in your styles using `@import '~invoker-tokens/index.scss';` and the same for others.

---

## Principles

### A11y First

A11ly is one of our main concerns when building products. Although we are still learning on how to make a fully accessible products, at least we can start with the easy one first, and that is contrast ratio of texts.

A low contrast text make it harder for people to read the content in your design. So, before you decide to use some colors for your design, make sure to have it tested first and comply with the WCAG standard.

You can use these browser-based tools to have your colors tested:

* [https://colorable.jxnblk.com](https://colorable.jxnblk.com)
* [https://contrastchecker.com](https://contrastchecker.com)
* [http://accessible-colors.com](http://accessible-colors.com)

The minimum contrast needed for your text to have good level of readibility or comply with the a11y standard is depend on it's size and weight. A bigger and bolder texts are easier to read, while a smaller text with thin weight needs a higher color contrast to have better readibility.

To have good readibility, the minimum requirement is to comply with contrast ratio of WCAG AA (>= 4.5) for **small-text** and WCAG AA Large (>=3.00) for **large-text**.

The term **Large-text** is for text with >= 18pt for regular weight, or text with size >= 14pt for bold weight. You can learn more about it [here](https://www.w3.org/TR/WCAG20/#larger-scaledef)

### Gestalt

Will add the content later, for now you can learn about gestalt principles [here](https://www.usertesting.com/blog/gestalt-principles/)

---

## Colors

### Brands

Communicate the brand colors using `brand-primary` and `brand-secondary` name. Usually 2 main colors is enough, but if you really need to push the limit, make it to `brand-tertiary`.

#### Brand Primary

```scss
$brand-primary-100 // Default for large text
$brand-primary-200 // Default for small text
$brand-primary-300 // Hover and tap
```

![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/sea-100.png "Sea 100 - #37A4A0")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/sea-200.png "Sea 200 - #008380")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/sea-300.png "Sea 300 - #00514F")

#### Brand Secondary

```scss
$brand-secondary-100  // Default for large text
$brand-secondary-200  // Default for small text
$brand-secondary-300  // Hover and tap
```

![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/scarlet-100.png "Scarlet 100 - #FD5C63")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/scarlet-200.png "Scarlet 200 - #D43242")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/scarlet-300.png "Scarlet 300 - #9A202C")

#### Accents Colors

Below is some pre-defined and a11y tested accents colors that you can use in your projects.

##### JEANS

```scss
$brand-jeans-100
$brand-jeans-200
$brand-jeans-300
```

![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/jeans-100.png "Jeans 100 - #5773C2")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/jeans-200.png "Jeans 200 - #3F46AD")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/jeans-300.png "Jeans 300 - #182385")

##### PLUM

```scss
$brand-plum-100
$brand-plum-200
$brand-plum-300
```

![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/plum-100.png "Plum 100 - #A18DAD")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/plum-200.png "Plum 200 - #866D96")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/plum-300.png "Plum 300 - #51425B")

##### SAGE

```scss
$brand-sage-100
$brand-sage-200
$brand-sage-300
```

![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/sage-100.png "Sage 100 - #56A472")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/sage-200.png "Sage 200 - #2C864C")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/sage-300.png "Sage 300 - #1B512E")

##### SKY

```scss
$brand-sky-100
$brand-sky-200
$brand-sky-300
```

![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/sky-100.png "Sky 100 - #4A9BDA")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/sky-200.png "Sky 200 - #267ABC")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/sky-300.png "Sky 300 - #184C75")

### Darks

> Mainly for Text colors

All `dark colors` are tested with white background `#FFFFFF` and comply with the a11y contrast ration WCAG AA. For usage with bacgkround color other than white, please do some test on your own.

```SCSS
// Colors using alpha value.
// Preferable!
$dark-alpha-90
$dark-alpha-80
$dark-alpha-70
$dark-alpha-60
$dark-alpha-50
// Lighter dark color -- For Borders and Shadow
$dark-alpha-40
$dark-alpha-30
$dark-alpha-20
$dark-alpha-10

// HEX Value
// Use this when you are sure about it or when it's necessary, i.e. alpha value not widely supported for developing HTML email
$dark-hex-90 // Headings
$dark-hex-80 // Headings and Body texts in text-heavy page such as blog post
$dark-hex-70 // Body texts
$dark-hex-60 // Captions and subtitles
$dark-hex-50 // Icons
// Lighter dark color -- For Borders and Shadow
$dark-hex-40
$dark-hex-30
$dark-hex-20
$dark-hex-10
```

![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/dark-90.png "Dark 90 - #0F0F0F")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/dark-80.png "Dark 80 - #292929")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/dark-70.png "Dark 70 - #484848")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/dark-60.png "Dark 60 - #767676")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/dark-50.png "Dark 50 - #8F8F8F")

### Light

```SCSS
// Colors using alpha value.
// Preferable!
// ALPHA
$light-alpha-100
$light-alpha-90
$light-alpha-80
$light-alpha-70
$light-alpha-60
$light-alpha-50
$light-alpha-40
$light-alpha-30
$light-alpha-20
$light-alpha-10

// HEX
$light-hex-100
$light-hex-90
$light-hex-80
$light-hex-70

```

### Tone

#### Danger

```scss
$tone-danger-100 // Use for Danger Background or Large text
$tone-danger-200 // Default for small text
$tone-danger-300 // Hover, active, focus and tap
```

![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/rose-100.png "Rose 100 - #FD5C63")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/rose-200.png "Rose 200 - #ED0001")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/rose-300.png "Rose 300 - #B50008")

#### Warning

> Only use these palettes as background color and use at least `$dark-60` as text for the warning.

```scss
$tone-warning-100
$tone-warning-200
$tone-warning-300
```

![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/amber-100.png "Amber 100 - #FFE380")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/amber-200.png "Amber 200 - #FFAB00")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/amber-300.png "Amber 300 - #FF8B00")

#### Success

```scss
$tone-success-100 // Use for success background
$tone-success-200 // Default for small text
$tone-success-300 // Hover, active, focus and tap
```

![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/verdant-100.png "Verdant 100 - #57D9A3")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/verdant-200.png "Verdant 200 - #00875A")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/verdant-300.png "Verdant 300 - #006644")

### Backgrounds

> Use these colors for background only.

Here are the sets of colors that you can use as background colors in your project.

All the background colors already tested and comply with contrast ratio **WCAG AA** for usages with `$dark-70`, `$dark-80`, and `$dark-90` texts.
If you want to use them with `$dark-50` text, you can see the test result on each card.

### Dust

```scss
$bg-dust-100
$bg-dust-200
$bg-dust-300
```

![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-dust-100.png "Dust 100 - #F7F7F5")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-dust-200.png "Dust 200 - #F0F0EE")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-dust-300.png "Dust 300 - #B7B7AD")

### Rose

```scss
$bg-rose-100
$bg-rose-200
$bg-rose-300
```

![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-rose-100.png "Rose 100 - #FCE7DD")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-rose-200.png "Rose 200 - #E3CDD1")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-rose-300.png "Rose 300 - #D8BAC0")

### Scarlet

```scss
$bg-scarlet-100
$bg-scarlet-200
$bg-scarlet-300
```

![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-scarlet-100.png "Scarlet 100 - #FFEAEE")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-scarlet-200.png "Scarlet 200 - #FFC4CF")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-scarlet-300.png "Scarlet 300 - #FFA2B3")

### Sea

```scss
$bg-sea-100
$bg-sea-200
$bg-sea-300
```

![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-sea-100.png "Sea 100 - #D7EFEE")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-sea-200.png "Sea 200 - #A9DCD7")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-sea-300.png "Sea 300 - #92D3CC")

### Plum

```scss
$bg-plum-100
$bg-plum-200
$bg-plum-300
```

![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-plum-100.png "Plum 100 - #DFD8E3")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-plum-200.png "Plum 200 - #D4D0E3")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-plum-300.png "Plum 300 - #BEB8D5")

### Sage

```scss
$bg-sage-100
$bg-sage-200
$bg-sage-300
```

![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-sage-100.png "Sage 100 - #E8F3EC")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-sage-200.png "Sage 200 - #CAD8B4")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-sage-300.png "Sage 300 - #B7CA9A")

### Sky

```scss
$bg-sky-100
$bg-sky-200
$bg-sky-300
```

![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-sky-100.png "Sky 100 - #E2EFF9")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-sky-200.png "Sky 200 - #B7D7F0")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-sky-300.png "Sky 300 - #91C2E8")

### Verdant

```scss
$bg-verdant-100
$bg-verdant-200
$bg-verdant-300
```

![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-verdant-100.png "Verdant 100 - #E4FDEB")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-verdant-200.png "Verdant 200 - #D9FCE3")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-verdant-300.png "Verdant 300 - #A9EEBC")

### Banana

```scss
$bg-banana-100
$bg-banana-200
$bg-banana-300
```

![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-banana-100.png "Banana 100 - #FFFDDD")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-banana-200.png "Banana 200 - #FFFBBB")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-banana-300.png "Banana 300 - #FFFE95")

### Sand

```scss
$bg-sand-100
$bg-sand-200
$bg-sand-300
```

![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-sand-100.png "Sand 100 - #F6F1E4")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-sand-200.png "Sand 200 - #E0D0B7")
![alt-text](https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/colors/bg-sand-300.png "Sand 300 - #D8C4A5")

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

[cover]: https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/cover-alt.png "Invoker Styles"
[mission]: https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/mission.png "Invoker Styles"

<!-- SPACES -->
[space-steps]: https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/space-steps.png "Space Steps"
[space-inset]: https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/space-inset.png "Space Inset"
[space-stack]: https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/space-stack.png "Space Stack"
[space-inline]: https://raw.githubusercontent.com/meridianid/invoker-styles/master/docs/space-inline.png "Space Inline"
