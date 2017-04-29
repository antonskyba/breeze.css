# ![Breeze.css](https://habrastorage.org/files/7e6/c78/6fc/7e6c786fcccc4e61a4c921b4e2ab47f7.png)
_Framework that inspires on writing better CSS_


## About

Breeze is lightweight, scalable, Stylus-based framework for medium and large web projects. It is not a set of designed UI elements, but instead it provides you with a ready-to-use architectural solution that helps to quickly bootstrap a project without worrying about basic things.

## Installation

Breeze is not available on Npm or Bower, therefore you have to download the source folder and put it into your project's styles folder. 

## Getting started

1. Set up most important Breeze variables.

   - Open `app.styl` and find the `$css-path` variable. By default majority of styles are located in the same folder as  the main file, but in case if you want to keep them separately assign to this variable path to your styles folder.  
  
   - Open `core.settings.styl` and choose your Base Unit and Base Ratio values. You will find description of these units and few useful links that may help you make your choice.  

2. Button example.

   Quickly overview `example.button.components.styl`. This is just an example file that shows you how it fits into the Breeze framework, but you may leave it and customize for your project needs.  
   

> **Note:** Breeze uses most recent version of Normalize.css that is available during the latest major framework update, but if you want to receive Normalize updates through Bower or Npm delete `normalize.generic.styl`, add Normalize.css as a dependency to your project and import it to the `app.styl`.

## Core framework ideas

#### Make CSS maintainable again

Under the hood Breeze uses so-called Inverted Triangle CSS (ITCSS): method of CSS-code organisation that will keep your project styles easy to maintain through whole development process.

#### Coherence & consistency

To reduce amount of magic numbers and rationalise most of values, you will find Base Unit and Base Ratio principles in framework's core. 

#### Lightweightness & compatibility

Breeze does not impose you with any restrictions and made so **it doesn't exclude usage of any other CSS tool or framework**.
