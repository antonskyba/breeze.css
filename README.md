# ![Breeze.css](https://habrastorage.org/files/ede/685/cf4/ede685cf4074400a8523cb34c94809d2.png)

**Better way to write CSS**

Breeze is lightweight, scalable, Stylus-based framework for medium and large web projects. It is not a set of designed UI elements, but instead it provides you with robust architectural solution that helps to quickly bootstrap a project without worrying about basic things.

## Core ideas

#### Maintainable styles

Under the hood Breeze uses so-called Inverted Triangle CSS (ITCSS): method of CSS-code organisation that will keep your project styles easy to maintain through whole development process.

#### Coherence & consistency

To reduce amount of magic numbers and rationalise most of values, you will find Base Unit and Base Ratio principles in framework's core.

#### Lightweightness & compatibility

Breeze does not impose you with any restrictions and made so **it doesn't exclude usage of any other CSS tool or framework**.

## Project Structure

Breeze follows special method of CSS-code organisation that keeps styles maintainable through whole development process, even after many years of development. The principle is quite simple but powerful and lies in separating code into different layers:

  - `/config`: global files that contain things that need to be made available to the entire codebase: variables and miscellaneous settings.
  - `/functions`: globally used functions and mixins.
  - `/generic`: low-specific & far-reaching rulesets: reset, normalize, box-sizing definition, etc.
  - `/html-tags`: styles for unclassed HTML elements (e.g. `<body>`, `<input>`, etc).
  - `/objects`: class-based selectors which define objects, abstractions, and design patterns.
  - `/ui-components`: discrete, complete chunks of UI.
  - `/utilities`: utilities and helper classes with ability to override anything which goes before.

## Base Unit & Base Ratio

The purpose of it is to establish an effective system to guide decision-making about sizing, scale and proportion throughout the project. The rules and governing principles set out here for the system typography ripple out and inform all UI construction from this point — layouts grids, column widths, tables, margins — everything reads from the same hymn sheet. Done with care and skill this ultimately creates a solid underlying aesthetic structure and results in a rhythmic, harmonious and cohesive design.  

## Measurement Units

Breeze uses `rem` units for almost everything, but `em` in places where it's needed to depend on `font-size`. Pixel units are only used in rare places, like debugging utilities. Such approach gives you maximum flexibility & functionallity, as well as ability to use all power of CSS.

## Namespaces

All classes in Breeze has specific prefixes which explicitly tell you what layer they belong to:

  - `.o-`: objects
  - `.c-`: ui-components
  - `.u-`: utilities

Be sure to follow this convention in your own code as well to keep a consistent naming convention across your code base. 

If you want to dive deeper into namespacing classes and want to know why this is a great idea, have a look at [this article](http://csswizardry.com/2015/03/more-transparent-ui-code-with-namespaces/).

## Responsive

Breeze comes with responsive functionality for some modules and uses [Rupture](https://github.com/jescalan/rupture) as a main tool for providing that.

## Installation

Breeze is not available on Npm or Bower, therefore you have to download the source folder and put it into your project's styles folder.

## Getting started

1. Open `app.styl` and find the `$css-path` variable. By default style files are located together with `app.styl`, but in case if you want to keep them separately assign to this variable your custom path.

2. Open `_base.config.styl` and choose your Base Unit and Base Ratio values. You will find a brief description of each of these units and few useful links that may help you to make a choice.

> **Note:** Breeze uses most recent version of Normalize.css that is available during the latest major framework update, but if you want to get Normalize updates through Bower or Npm delete `normalize.generic.styl`, add Normalize.css as a dependency to your project and import it to the `app.styl`.
