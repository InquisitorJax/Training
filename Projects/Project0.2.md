# Level 0 Project 2

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
 All the rest has been done for you. When you click on the list, that item will be the selcted object and it's details displayed.

 The data is defined in the staff-data, also in the resources folder. You will notice that the "unknown" record has more fields defined and thus should show more details that the others.
 
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
 
## Note
The styling as sefined in the mockup and that you see when doing this project might not match up in some cases. 
You don't have to worry about that. These may include things like checkbox background colors and required items having a red * next to the title. The purpose of this excersize is familiarize yourself with the schema mechanincs on how to put togeather a schema to be used in the dynamic screen mechanism. The styles will change and be updated over time so don't worry about it when colors don't match.

Your project must have one tab on it.
Some group items have headers ("HEADER", "PERSONAL DETAILS", .... These headers you can make h2 elements.

When defining the field maps in the schema, use a 1:1 relation with the property defined in the model.
```
 {
     "field": "firstName",
     "map": "firstName"
 }
```


