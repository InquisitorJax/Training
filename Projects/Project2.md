# Project 2

## Introduction
Rewrite Project 1 using web project assist.
Get a binary from pragma.

All classes and custom components must use be created through web project assist.
Please note that this will also create tests for you to maintain and extend.

The application should be tested on multiple browsers on different devices.
This includes firefox, chrome on desktop. Test the application on atleast one mobile device.
The application layout must be responsive and work perfectly on all devices as present in chrome dev tools.

Hint: you will need to use media queries.

Please note that this project must also be added to github please.

## Global packages you must have installed
1. build-utilities-commandline
1. http-server
1. jspm

To install a global package use the following command

`npm install -g <packagename>` e.g. `npm install -g jspm`

## Starting a new project
To create a new project: 
1. Create a project folder.
1. Using [build-utilities-commandline](https://github.com/pragmaproducts/build-utilities-commandline), select that folder and create a new project.

## Technology 
From this point you will start using supporting technologies.

1. Sass for css development

You will also start writing tests for your projects must have a keen understanding of:

1. Mocha
2. Chai
3. Sinon

The user interface part of the application uses aurelia as the framework.
http://aurelia.io/

If you need a reference on the Aurelia api you can look at their cheat sheet.
http://aurelia.io/hub.html#/doc/article/aurelia/framework/latest/cheat-sheet

## NB
Please use web project assist to create the classes for your project.

## Goals
Take what you have learned and make it a practical application.

### Features required
All the same Project 1 features are expected.
In addition to that we require:

1. Proper UI styling using Sass
2. 90% test coverage
3. All audits to pass on all code and html.

See the build utilities wiki for more details on the what auditing is available.

### Designs
Please follow the following designs for [mobile](https://github.com/pragmaproducts/Training/blob/master/Images/project2-mobile.png) and [desktop](https://github.com/pragmaproducts/Training/blob/master/Images/project2-desktop.png)

1. Please make note of the styling differences between not selected, selected and done items.
1. The add button is a normal button styled to look round, no graphics used except for the + svg icon used in the middel.
1. If you have difficulty styling the checkboxes to look as per the design you can leave them as normal checkboxes.
The done item however must not have  checkbox but a checked svg image.