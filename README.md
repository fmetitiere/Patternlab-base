# PatternLab Scalio Base

## Overview

This is an improved version of [PatternLab Node Edition Gulp](https://github.com/pattern-lab/edition-node-gulp) with SASS compilation included.

### Requirements

The (main) requirement for running this project is [Node](https://nodejs.org) and [NPM](https://www.npmjs.com) (which usually comes when installing Node).

The recommended way to have NPM installed is via [NVM](https://github.com/creationix/nvm#installation) which will also allow you to have different versions installed at the same time.

You do not need this, as you will see later.

If you're stumbling on any error, have a look at the [troubleshooting section](#Troubleshooting) below

### Installation

Clone the current repo:

    $ git clone https://github.com/fmetitiere/Patternlab-base.git
    $ cd patternlab-base-scalio

Install all the dependencies:

    $ yarn

Run the project:

    $ yarn start

You can now access the website at <http://localhost:3000>.

### SASS compilation

The `gulpfile.js` will automatically compile, inject, and reload the browser upon changes to any of the `*.scss` files available in the directory `/source/sass/`.

The current version now includes [normalize](https://necolas.github.io/normalize.css/), albeit [its SASS version](https://github.com/JohnAlbin/normalize-scss), and [autoprefixer](https://github.com/postcss/autoprefixer) to automate vendor prefixes.

