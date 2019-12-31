![Cryb OSS](.github/cryb.png "Cryb OSS Logo")

_**Borealis**<sup>BETA</sup> — CSS framework_

[![GitHub contributors](https://img.shields.io/github/contributors/crybapp/borealis)](https://github.com/crybapp/borealis/graphs/contributors) [![License](https://img.shields.io/github/license/crybapp/borealis)](https://github.com/crybapp/borealis/blob/master/LICENSE) [![Patreon Donate](https://img.shields.io/badge/donate-Patreon-red.svg)](https://patreon.com/cryb)

## Docs
* [Info](#info)
    * [Status](#status)
* [Codebase](#codebase)
    * [Folder Structure](#folder-structure)
    * [First time setup](#first-time-setup)
        * [Installation](#installation)
    * [Compiling CSS locally](#compiling-css-locally)
* [Questions / Issues](#questions--issues)

## Info
`@cryb/borealis` is the CSS framework for all Cryb web apps.

It uses [Sass](https://sass-lang.com/) as the core preprocessor.

### Status
`@cryb/borealis` has been actively developed since December 2019.

## Codebase
The codebase for `@cryb/borealis` is written in Sass.

### Folder Structure
```
cryb/borealis/
├──┐ src # The core source code
│  ├── components # Config files for Redis, Passport, etc
│  └── utils # Static 
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
