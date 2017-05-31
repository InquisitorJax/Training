# Project 0

## Introduction
 Before you get started with anything you need to understand what is required to create templates for the dynmaic runtime screengen.
 
 Fork and implement the design for:  
 https://github.com/pragmaproducts/pragma-screengen
 
 ## Implementing the screen
 You only need to make changes to one file.
 The src/resources folder contains a staff-template.js file.
 https://github.com/pragmaproducts/pragma-screengen/blob/master/src/resources/staff-template.js
 
 Make changes to this file so that the design found in developer notes is implemented.
 
 ## Getting started
 1. Read the template document to understand the schema rules  
 https://github.com/pragmaproducts/pragma-views/blob/master/developer-notes/template-parser.md
 1. Experiment with a single tab to get comfortable on how the parts fit.
 1. Implement the remainder of the screen.
 
 ## Viewing your changes
 There are two terminal commands you need to know to build the project and spawn a server to view those changes.
 
 1. `gulp build:all`
 2. `gulp serve`
 
 Note that the server will run until you kill it in terminal, closing the browser does not stop the server.
 
 Clear cache and hard reload page using
 ctrl + shift + r on windows and 
 cmd + shift + r on mac
 
 ## HTML
 If you need html elements that are not supported by default, you can use this cheatsheet as a reference:  
 https://github.com/pragmaproducts/Training/blob/master/Cheatsheets/HTML5-cheat-sheet.pdf
 
## CSS Classes you may need
 There are not many scenarios where you will need to apply styling. You certainly don't have to create any css classes yourself.
 The following classes already exist for you to use.
 
 1. container
 1. vertical
 1. horizontal
 1. stretch
 1. default-padding
 1. default-padding-left
 1. default-padding-right
 1. default-padding-bottom
 1. checkbox-composite
 
 CSS details can be found at:  
 https://github.com/pragmaproducts/pragma-views/tree/master/sass/lib.
 
 In particular you can look at:  
1. Layout
 1. Mixins
 