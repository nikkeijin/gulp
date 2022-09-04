# Frontend Development Workflow with PUG, SASS and JS

PUG:
Will compile the content of index.pug into layout.pug and generate a index.html file that we can view in the browser.

* layout.pug - file that loads our compiled CSS & JavaScript

SASS:
Will create a /dist/assets folder with a single style.css file that contains the compiled CSS

* _global.scss – some styles for the body element using the variables
* _vars.scss – defines SASS variables to use
* style.scss – imports the other “partial” scss files

JavaScript:
Will be concatenating multiple JavaScript files into a single file named script.js that is located in the /assets folder along with the compiled CSS.

# Must have node, npm, and npx to use gulp.

Homebrew:
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Node with NPM
```
brew install node
```

# Gulp command line utility

```
npm install gulp-cli --global
```

# Starting a project

create the project directory and run npm init:
```
npm init -y
```

Gulp can then be installed into our project with the following command:
```
npm install gulp --save-dev
```

Plugins:
```
npm install sass gulp-sass --save-dev

npm install gulp-concat --save-dev

npm install gulp-pug --save-dev

```

Watch files for changes:
```
gulp watch
```
