# Configuring Webstorm 

It is often usefull to test your code by placing breakpoints in your code. This document will describe to you how to configure your webstorm to allow for better testing.
Please note that this document assumes you will be using build-utilities-commandline in your project though it is not required for the content of this document.

## Configure testing with code coverage
ALl these changes will be made in your package.json file at the root of your project.  
You will need the following packages installed using npm. The easiest way to install them is to copy the text below and past it as part of your devDependencies.

```
"babel-core": "^6.24.1",
"babel-preset-es2015": "^6.24.1",
"babel-plugin-istanbul": "^4.1.3",
"babel-plugin-transform-class-properties": "^6.24.1",
"babel-plugin-transform-decorators-legacy": "^1.3.4",
"chai": "^3.5.0",
"istanbul": "^0.4.5",
"mocha": "^3.4.2",
"nyc": "^10.3.2",
"sinon": "^2.3.1"
```

After you have added this to your devDependencies and saved the package.json file you can run `npm install`. Please note that if you have any install issues, you may need to delete the 'package-lock.json' file if it exists in the root of the project.

As an alternative you can manully install these items one for one using `npm install --save-dev packagename`

You can now add this item to the scripts property of the package.json file.

```
"test": "nyc mocha --compilers js:babel-core/register --recursive"
```

you will also need to add the following to the root of the package.json configuration

```
  "babel": {
    "presets": [
        "es2015"
    ],
    "plugins": [
        "transform-decorators-legacy",
        "transform-class-properties"
    ]
  },
  "nyc": {
    "check-coverage": true,
    "require": [
      "babel-register"
    ],
    "reporter": [
      "lcov",
      "text-summary"
    ],
    "include": [
      "src/**/*.js"
    ],
    "exclude": [
      "app/**/*.*",
      "node_modules/**/*.*",
      "jspm_packages/**/*.*"
    ],
    "cache": true,
    "all": true
  }
```

When you run the test script it will now do testing and code coverage of your files. It will transpile both your tests and code from ES6 before running the tests.
When the tests are done running it will create a coverage folder at the root of your project containing a index.html file describing the detailed coverage of your code.
