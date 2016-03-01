## Wut?

This is a CSS layout "library" based on [flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Using_CSS_flexible_boxes) inspired entirelly by [Angular Material's layout system](https://material.angularjs.org/latest/layout/introduction) ([repo](https://github.com/angular/material/)), so **they are the cool guys**.

It is written in [Stylus, a CSS preprocessor](http://stylus-lang.com/) using [autoprefixer-stylus](https://www.npmjs.com/package/autoprefixer-stylus), a tool that adds all the annoying vendor prefixes for our CSS properties.

A minified & vendor prefixed CSS file is included in the repo inside ./dist folder.


## Install the dependencies

Here I assume you have [NodeJS installed](https://nodejs.org/en/download/) already, like every cool kid on the block.

First you'll need to install Stylus globally:

`npm install -g stylus`

Then you'll need to install autoprefixer-stylus because we live in a diverse world and _all_ browsers like to read CSS in a different way:

`sudo apt-get install -g autoprefixer-stylus`

**Note**: you can skip this step if you don't plan to support all current browsers, or if you come from a distant future where CSS is unified and no one uses old IE, in that case I hate you... I mean, I love you! can you use one of those Tardis like machines to get me there?

## Working with stylus

#### To play around with the lib:

`stylus -u autoprefixer-stylus -w`

This starts a server watching for the specified file for changes and compiling it

    
#### To generate a minified & vendor prefixed version:

`stylus -u autoprefixer-stylus -c main.styl -o ./dist/main.css`

This updates the ./dist/main.css file.

