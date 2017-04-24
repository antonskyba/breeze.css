# Breeze.css
_Framework that inspires on writing better CSS_


## About

Breeze is lightweight, scalable, Stylus-based framework for medium and large web projects. It is not a set of designed UI elements, but instead it provides you with a ready-to-use architectural solution that helps to quickly bootstrap a project without worrying about basic things.

## Installation

Breeze is not available on Npm or Bower, therefore you have to download the project's source folder and put it into your project's styles folder. 

## Getting started

1. Set up most important Breeze variables.

   - Open app.styl and find the `$css-path` variable. Assign to this variable path to your styles folder in case if you want to keep `app.styl` and rest `*.styl` files in separate folders.  
  
   - Open `core.settings.styl` and choose your Base Unit and Base Ratio values. You will find description of these units and some useful links that may help you make your choice.  

2. example.button.components.styl.

   Quickly overview `example.button.components.styl`. This is just an example file that shows you how it fits into the Breeze framework, but you may leave it and customize for your project needs.  
   

> **Note:** Breeze uses most recent version of Normalize.css that is available during the latest major framework update, but if you want to receive Normalize updates through Bower or Npm delete `normalize.generic.styl`, add Normalize.css as a dependency to your project and import it to the `app.styl`.

## Core ideas

#### Make CSS maintanable again

Under the hood Breeze uses so-called Inverted Triangle CSS (ITCSS): method of CSS-code organisation that will keep your project styles easy to maintain through whole development process.

#### Coherence & consistency

To reduce amount of magic numbers and rationalise most of values, you will find Base Unit and Base Ratio principles in framework's core. 

#### Lightweightness & compatibility

Breeze does not impose you with any restrictions and made so **it doesn't exclude usage of any other CSS tool or framework**.
