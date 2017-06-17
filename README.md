# ![Breeze.css](https://habrastorage.org/files/ede/685/cf4/ede685cf4074400a8523cb34c94809d2.png)

**Framework that inspires on writing better CSS**

Breeze is lightweight, scalable, Stylus-based framework for medium and large web projects. It is not a set of designed UI elements, but instead it provides you with robust architectural solution that helps to quickly bootstrap a project without worrying about basic things.

## Core ideas

#### Keep styles maintainable

Under the hood Breeze uses so-called Inverted Triangle CSS (ITCSS): method of CSS-code organisation that will keep your project styles easy to maintain through whole development process.

#### Coherence & consistency

To reduce amount of magic numbers and rationalise most of values, you will find Base Unit and Base Ratio principles in framework's core.

#### Lightweightness & compatibility

Breeze does not impose you with any restrictions and made so **it doesn't exclude usage of any other CSS tool or framework**.

## Installation

Breeze is not available on Npm or Bower, therefore you have to download the source folder and put it into your project's styles folder.

## Getting started

1. Open `app.styl` and find the `$css-path` variable. By default style files are located together with `app.styl`, but in case if you want to keep them separately assign to this variable your custom path.

2. Open `_core.settings.styl` and choose your Base Unit and Base Ratio values. You will find a brief description of each of these units and few useful links that may help you to make a choice.

> **Note:** Breeze uses most recent version of Normalize.css that is available during the latest major framework update, but if you want to get Normalize updates through Bower or Npm delete `_normalize.generic.styl`, add Normalize.css as a dependency to your project and import it to the `app.styl`.