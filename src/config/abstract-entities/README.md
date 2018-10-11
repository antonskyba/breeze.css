### Abstract Entities

The module contains settings for components that share the same look & feel and therefore should have common variables. For example, you have some textfield that has a height equal to 40px and some third-party library for dropdown select element that should have the same height equal to 40px. It is reasonable to create an abstract entity named 'form-control' and give it a height variable that equal to 40px and assign its variable to your textfield and dropdown select element to give them consistent look and have flexible contol over them.
