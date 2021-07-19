# PatternLab Scalio Base

## Overview

This is an improved version of [PatternLab Node Edition Gulp](https://github.com/pattern-lab/edition-node-gulp) with SASS compilation included.

Check out the [Technical Bits](#technical-bits) if you want to learn more about it.

## Setup and run

### Requirements

The (main) requirement for running this project is [Node](https://nodejs.org) and [NPM](https://www.npmjs.com) (which usually comes when installing Node).

The recommended way to have NPM installed is via [NVM](https://github.com/creationix/nvm#installation) which will also allow you to have different versions installed at the same time.

There's nothing wrong in using any other way to install Node, like the default system-installed Node version, as long as it's above version 5.0.

_Optionally, but not recommended_: once you have installed Node and NPM, you can install Gulp 4 globally, as follows:

    $ npm install -g gulpjs/gulp#v4.0.0

You do not need this, as you will see later.

If you're stumbling on any error, have a look at the [troubleshooting section](#Troubleshooting) below

### Installation

Clone the current repo:

    $ git clone git@bitbucket.org:digitalrigbitbucketteam/patternlab-base-toolkit.git
    $ cd patternlab-base-toolkit

Install all the dependencies:

    $ npm install

Run the project:

    $ npm start

You can now access the website at <http://localhost:3000>.

## Technical bits

There are some major differences from the original project, namely:

- SASS compilation
- Concatenation of PL styles (`pattern-scaffolding` files)
- Directory structure
- Improved code standards and linting used throughout the project

### SASS compilation

The `gulpfile.js` will automatically compile, inject, and reload the browser upon changes to any of the `*.scss` files available in the directory `/source/sass/`.

The current version now includes [normalize](https://necolas.github.io/normalize.css/), albeit [its SASS version](https://github.com/JohnAlbin/normalize-scss), and [autoprefixer](https://github.com/postcss/autoprefixer) to automate vendor prefixes.

