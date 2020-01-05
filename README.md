![Cryb OSS](.github/cryb.png "Cryb OSS Logo")

_**Borealis**<sup>BETA</sup> — CSS framework_

[![GitHub contributors](https://img.shields.io/github/contributors/crybapp/borealis)](https://github.com/crybapp/borealis/graphs/contributors) [![License](https://img.shields.io/github/license/crybapp/borealis)](https://github.com/crybapp/borealis/blob/master/LICENSE) [![Patreon Donate](https://img.shields.io/badge/donate-Patreon-red.svg)](https://patreon.com/cryb)

## Docs
* [Info](#info)
    * [Features](#features)
        * [Planned Features](#planned-features)
    * [Status](#status)
* [Installation](#installation)
	* [CDN](#cdn)
* [Usage](#usage)
	* [HTML](#html)
	* [Nuxt.js](#nuxt.js)
* [Codebase](#codebase)
    * [Folder Structure](#folder-structure)
    * [First time setup](#first-time-setup)
        * [Installation](#installation)
    * [Compiling CSS locally](#compiling-css-locally)
* [Questions / Issues](#questions--issues)

## Info
`@cryb/borealis` is the CSS framework for all Cryb web apps.

Borealis is built to unify UI design across our web app, admin panel, landing page and any future web apps we build. It is not intended to be used in non-Cryb applications, but feel free to do so.

It uses [Sass](https://sass-lang.com/) as its main preprocessor.

### Features
* Dark mode support

#### Planned Features
* Mobile support

### Status
`@cryb/borealis` has been actively developed since December 2019.

## Installation
This library is available on the [NPM registry](https://www.npmjs.com/package/@cryb/borealis). To install, run:
```bash
npm i @cryb/borealis --save
```
If you're using [Yarn](https://yarnpkg.com), run:

```bash
yarn add @cryb/borealis
```

### CDN
`@cryb/borealis` is also available through [unpkg](https://unpkg.com/) and [jsdelivr](https://www.jsdelivr.com/).

*Note: you only need to include one CSS file. Below we include both minified and unminified CDN links—we recommend that you use the minified version*

#### unpkg
```
# Minified
https://unpkg.com/@cryb/borealis@latest/css/borealis.min.css

# Uminified
https://unpkg.com/@cryb/borealis@latest/css/borealis.css
```

#### jsdelivr
```
# Minified
https://cdn.jsdelivr.net/npm/@cryb/borealis@0.0.3/css/borealis.min.css

# Unminified
https://cdn.jsdelivr.net/npm/@cryb/borealis@0.0.3/css/borealis.css
```

## Usage
Compiled CSS can be found under `@cryb/borealis/dist/` as `borealis.css` and `borealis.min.css`.

We recommend you use `borealis.min.css` in production environments.

### HTML
Simply link Borealis as you would any other HTML file:
```html
<head>
	<link rel="stylesheet" href="css/borealis.min.css">
</head>
```

Borealis is also offered through a CDN. While we recommend you download Borealis locally, you can use either [unpkg](https://unpkg.com/) or [jsdelivr](https://www.jsdelivr.com/).

#### unpkg
```html
<!-- Minified (production, recommended) -->
<link rel="stylesheet" href="https://unpkg.com/@cryb/borealis@latest/css/borealis.min.css" />

<!-- Unminified (development) -->
<link rel="stylesheet" href="https://unpkg.com/@cryb/borealis@latest/css/borealis.min.css" />
```

#### jsdelivr
```html
<!-- Minified (production, recommended) -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@cryb/borealis@0.0.3/css/borealis.min.css" />

<!-- Unminified (development) -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@cryb/borealis@0.0.3/css/borealis.css" />
```

### Nuxt.js
After installation, Borealis can be easily integrated into a Nuxt.js project through `nuxt.config.js`. See the example below:
```js
export default {
	css: [
		'@cryb/borealis'
	]
}
```

## Codebase
The codebase for `@cryb/borealis` is written in Sass.

### Folder Structure
```
cryb/borealis/
├──┐ src # Uncompiled Sass
│  ├── components # Buttons, boxes, etc
│  ├── pages # Styles for pages
│  └── utils # Static variables
├─── dist # Compiled CSS
└──┐ examples # Pages to test compiled CSS
   └── assets # Assets for example pages
```

### First time setup
First, clone the `@cryb/borealis` repository locally:

```
git clone https://github.com/crybapp/borealis.git
```

#### Installation
You also need to install the required dependencies by running `yarn`.

### Compiling CSS locally
To run `@cryb/borealis` in development mode, run `yarn dev`. This mode will watch for changes on `.sass` files under `dist/` and then compile accordingly.

Once you have finished your changes, run `yarn build` to fully compile to `dist/`. You should do this before committing.

## Questions / Issues
If you have an issues with `@cryb/borealis`, please either open a GitHub issue, contact a maintainer or join the [Cryb Discord Server](https://discord.gg/ShTATH4) and ask in #tech-support.
