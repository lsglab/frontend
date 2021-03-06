<p align="center"><img width=15% src="./.github/lsglogo.png"></p>
<h2 align="center">A shiny new frontend for our <a href="https://lsg.musin.de" target="_blank">school homepage</a></h2>
<p align="center">
  <a href="https://github.com/lsglab/frontend/"><img src="https://img.shields.io/github/license/lsglab/frontend?style=flat-square" alt='AGPLv3 licensed' /></a>
  <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
<a href='#contributors'><img src='https://img.shields.io/github/all-contributors/lsglab/frontend/master' alt='All-Contributors Count'></a>
<!-- ALL-CONTRIBUTORS-BADGE:END -->
</p>

## Overview

This is our new homepage written entirely in Svelte (using the Sapper framework). It will replace the outdated website visitors are currently greeted with.

## Setup

Clone this repository and you're good to go.  
Please note that scripts in this project might only work in a POSIX-compliant shell environment (located at `/bin/sh`); you'll be fine with most \*nix operating systems. More specifically, if you're on Windows ([m](https://tinyurl.com/nuub2bq)[y](https://tinyurl.com/y2emej63)[ ](https://tinyurl.com/y2lzznux)[c](https://tinyurl.com/y3v8vo5a)[o](https://tinyurl.com/y4qcfkw3)[n](https://tinyurl.com/y5gm9ysv)[d](https://tinyurl.com/y69uplwl)[o](https://tinyurl.com/yygc57ta)[l](https://tinyurl.com/yynoa7ql)[e](https://tinyurl.com/y3shavwn)[n](https://tinyurl.com/yxladmrj)[c](https://tinyurl.com/y3yxymqr)[e](https://tinyurl.com/y2c6alo5)[s](https://tinyurl.com/y5qtqr6p)), you'll need to spin up a better environment - WSL seems to be a good fit.  
While this certainly is not a requirement, [Visual Studio Code](https://code.visualstudio.com/) (or, even better, its open source release [VSCodium](https://vscodium.com/)) is highly recommended, since there are official extension recommendations and workspace settings in this repository for it. If you prefer a different editor (Atom, Vi*m*, Emacs...), you'll have to **install the necessary plugins** for svelte support, linting and formatting yourself. These tools are important as they save a lot of time and allow you to check and (auto)fix your commits locally before they pass tests during CI. You'll find a list of keywords to search for in your editors package manager in the [Tech stack](#tech-stack) section.

## Development

We use `package.json` scripts exclusively as a front-end for task automation, and **yarn instead of npm** as a package manager. [Rollup](https://rollupjs.org/) serves as our asset bundler. We use [Prettier](https://prettier.io/), [ESLint](https://eslint.org/) and [stylelint](https://stylelint.io/) to format all css, javascript, json and more automatically before commiting and when the editor saves (assuming the plugins are installed).

### Scripts

-   `yarn do:sync|do:commit|...`: These scripts are related to git operations, and are explained in the [Contributing](CONTRIBUTING.md) guide
-   `yarn do:dev`: Starts a hot-reloading development environment in `__sapper__/dev`
-   `yarn do:build`: Builds sapper in the `__sapper__/build` directory for server-side serving
-   `yarn do:start`: Starts the server-side polka instance from `__sapper__/build`
-   `yarn do:export`: Builds a static sapper instance by snapshotting each hydratable page returned from the server
-   `yarn do:serve`: Serves the exported static webpage
-   `yarn do:autofix`: Automatically formats, lints and fixes all code
-   `yarn do:testing`: Formats, lints and tests; fails on error

## Tech stack

-   [Git](https://git-scm.com/) - Version control
-   [GitHub Actions](https://github.com/features/actions) - CI/CD
-   [GitPod](https://www.gitpod.io/) - reproducible dev environments
-   [NodeJS](https://nodejs.org/en/) - Server-side JavaScript
-   [Polka](https://github.com/lukeed/polka) - NodeJS web server
-   [Svelte](https://svelte.dev/) - modern JavaScript compiler
-   [Sapper](https://sapper.svelte.dev/) - official Svelte framework
-   [Yarn](https://yarnpkg.com/) - Package management
-   [Rollup](https://rollupjs.org/) - Bundler
-   [Cypress](https://www.cypress.io/) - UI testing
-   [Editorconfig](https://editorconfig.org/) - IDE file style consistency
-   [Prettier](https://prettier.io/) - Code formatting
-   [ESLint](https://eslint.org/) - JavaScript linting
-   [Stylelint](https://stylelint.io/) - CSS style linting
-   [Vercel](https://vercel.com/) - Automatic deployments

## Contributing

There is a contribution guide in [CONTRIBUTING.md](CONTRIBUTING.md) detailing the git workflow in this repository. We do [Trunk based development](https://trunkbaseddevelopment.com/).

## Contributors ✨

Special thanks go to these contributors. We follow the [all-contributors](https://allcontributors.org/) specification ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="https://github.com/GitGangGuy"><img src="https://avatars0.githubusercontent.com/u/50679178?v=4" width="100px;" alt=""/><br /><sub><b>GitGangGuy</b></sub></a><br /><a href="https://github.com/lsglab/frontend/commits?author=GitGangGuy" title="Code">💻</a> <a href="https://github.com/lsglab/frontend/issues?q=author%3AGitGangGuy" title="Bug reports">🐛</a> <a href="https://github.com/lsglab/frontend/commits?author=GitGangGuy" title="Documentation">📖</a> <a href="#projectManagement-GitGangGuy" title="Project Management">📆</a> <a href="#plugin-GitGangGuy" title="Plugin/utility libraries">🔌</a> <a href="#content-GitGangGuy" title="Content">🖋</a> <a href="#design-GitGangGuy" title="Design">🎨</a> <a href="#ideas-GitGangGuy" title="Ideas, Planning, & Feedback">🤔</a></td>
    <td align="center"><a href="https://github.com/Flosi23"><img src="https://avatars1.githubusercontent.com/u/56218180?v=4" width="100px;" alt=""/><br /><sub><b>Flosi23</b></sub></a><br /><a href="https://github.com/lsglab/frontend/commits?author=Flosi23" title="Code">💻</a> <a href="#content-Flosi23" title="Content">🖋</a> <a href="#design-Flosi23" title="Design">🎨</a> <a href="#ideas-Flosi23" title="Ideas, Planning, & Feedback">🤔</a></td>
    <td align="center"><a href="https://github.com/jamwag"><img src="https://avatars3.githubusercontent.com/u/42468118?v=4" width="100px;" alt=""/><br /><sub><b>James Wagner</b></sub></a><br /><a href="https://github.com/lsglab/frontend/commits?author=jamwag" title="Code">💻</a> <a href="#content-jamwag" title="Content">🖋</a> <a href="#design-jamwag" title="Design">🎨</a> <a href="#ideas-jamwag" title="Ideas, Planning, & Feedback">🤔</a></td>
    <td align="center"><a href="https://github.com/Lacrimus"><img src="https://avatars1.githubusercontent.com/u/55695243?v=4" width="100px;" alt=""/><br /><sub><b>Lacrimus</b></sub></a><br /><a href="#ideas-Lacrimus" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/lsglab/frontend/commits?author=Lacrimus" title="Code">💻</a></td>
  </tr>
</table>

<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

Contributions of any kind are welcome!
