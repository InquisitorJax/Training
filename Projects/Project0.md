# Project 0

## Introduction
 Before you get started with anything you need to understand what is required to create templates for the dynmaic runtime screengen.
 
 Fork and implement the design for:  
 https://github.com/pragmaproducts/pragma-screengen
 
 ## Getting started
 1. Read the template document to understand the schema rules  
 https://github.com/pragmaproducts/pragma-views/blob/master/developer-notes/template-parser.md
 1. Install package dependencies by running the following commands on the root of the project  
 2.1 npm install  
 2.2 jspm install -y
 1. Experiment with a single tab to get comfortable on how the parts fit.
 1. Implement the remainder of the screen.
 
 ## Implementing the screen
 You only need to make changes to one file.
 The src/resources folder contains a staff-template.js file.
 https://github.com/pragmaproducts/pragma-screengen/blob/master/src/resources/staff-template.js
 
 Make changes to this file so that the design found in developer notes is implemented.
 
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
 
