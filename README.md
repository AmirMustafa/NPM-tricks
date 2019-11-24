# NPM-tricks
This repository just shares the all the commands in npm and tricks

## Explainations

Node Package Manager
====================

1.  Check installed or not: npm -v in terminal

INSTALL NPM:
For this you need to install node.

For windows: Install node software. Npm will be installed
For Linux:  ``` sudo apt install nodejs ```

--------------------------------------------------------------------------------------------------

COMMANDS IN NPM
================
A> UPDATE NPM AND HELP COMMANDS
-------------------------------
1. npm install npm@latest -g       // updates npm package
2. npm help                        // get all the commands of npm

B> INITIALIZE THE PACKAGE
----------------------
3. npm init                        // initialize the package.json file      
4. npm init -y                     // sets default value without asking

5. npm config list                 // get all the config name
6. npm config list -l              // get all the config name

C> NPM CONFIGURATION
---------------------
7. Suppose when you want to run npm init- y  and you want to add author name as your name which initially comes empty

a. SET KEYWORD

npm config set init-author-name "Amir Mustafa"

Now you run point 4 in package.json it will be generated with the name entered

b. GET KEYWORD
npm config get init-author-author-name

c. EDIT CONFIG list
npm config list
npm config list -l  // get full list details

d. To edit npm file globally
npm config edit --global

e. DELETE KEYWORD
npm config delete <keyword>
npm config delete init-author-name

----------------------------------------------------------------------------------------------
CHECK PACKAGE NAME 
===================

https://www.npmjs.com/

----------------------------------------------------------------------------------------------

INSTALL PACKAGE
===============

npm install <package-name>

eg.
npm install lodash          // Basic way
npm install lodash@latest   // Get the latest version
npm install lodash@2.1.1    // Get the specific version
npm i lodash                // i keyword instead of install
npm i lodash --save-dev     

--save-prod or -P       // By default
--save-dev or -D        //  Package will appear in your devDependencies
--save-optional or -O   // Package will appear in your optionalDependencies
--no-save               // Prevents saving to dependencies

- devDependencies - These are dependencies which may not required in production

----------------------------------------------------------------------------------------------

package.json vs package-lock.json
==================================

Both file are almost same. Suppose we create a project package with v1. Say we installed lodash.
After some time when lodash new version is available and this project is installed in some other computer. It may show confliction

So package-lock.json contains exact version at the time of development. So ot will intall specific version at the time project was developed
----------------------------------------------------------------------------------------------

INSTALL PACKAGE
-----------------

Suppose you have package.json file will all dependencies. To get all the package in node_modules

npm install

UPDATE PACKAGE
--------------
some of the ways to update:

Suppose package.json files is updated manually
npm update package
npm upgrade package
npm up package


DELETE A PACKAGE
------------------
some of the ways to update:

npm uninstall lodash
npm remove lodash --save
npm rm lodash 
npm r lodash
npm un lodash
npm unlink lodash
----------------------------------------------------------------------------------------------

OPEN OFFICIAL SITE OF The PACKAGE
==================================

npm docs <package_name>
npm docs lodash
----------------------------------------------------------------------------------------------

GET LIST OF PACKAGE INSTALLED IN YOUR CURRENT NPM
=================================================

npm ls  // gives list in tree format

-----------------------------------------------------------------------------------------------

START
======
npm start - This executes the command written in start property of the package.json file 
eg in react we start by typing 

npm start - this executes react-scripts start command


