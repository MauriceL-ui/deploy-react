# This folder contains all source files used to build the final scripts required by the web app (see assets folder) 

##This app makes use of the following:
- React, React Router, Flux, jQuery, Twitter Bootstrap, etc. for ultra-responsive UI development  
- Browserify bundling 
- Gulp build that:  
-- compiles JSX  
-- lints JSX and JS via ESLint  
-- bundles JS and CSS files  
-- publishes the built app files to the assets folder  
-- runs a dev webserver  
-- opens your browser at the dev URL  
-- reloads the browser upon save of source files  

Note that this full dev setup is not required, but makes life, development and updates much easier.  
You may not want the live reloading on the non-MAMP test webserver, for example.  Feel free to edit gulpfile.js to taste.
Currently setup for both a dev (containing debug JS) and release (all minified and good to go) build.

Also note that the app was originally written with React 0.13 using ES5 syntax. We do not currently have the time to rewrite it completely in ES2015 (ES6) syntax, 
but some code has been rewritten in ES6 where upgrades and updates were necessary (including moving to later versions of React and React Router).

##To setup dev environment:  
1. Install NodeJS (http://www.nodejs.org)  
2. Open any command line and cd to this directory  
3. `npm install` - Installs packages
4. `npm install -g gulp-cli` - Installs gulp globally
5. `gulp` - Builds the project and opens your browser. (Navigate to http://localhost:9005/ if your browser doesn't open automatically.)
