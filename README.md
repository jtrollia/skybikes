# SkyBikes
Bicycle rental program prototype :bike:

Demo [here](https://skybikes.jeanloup.me/)

![circle ci passing](https://circleci.com/gh/Malivuk/sky-bikes.svg?style=shield&circle-token=2f8aa2cdabc83b4b39fb99eb3e46bf812ab74c85)
[![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg)](http://standardjs.com)

## Installation

### Requirements
* node
* browser scope
* local storage
* session storage

### Scripts available
* install
* start (dev)
* build (prod)
* test (manually)

### How to use
* register
* login as random
* log as admin
* log as worker

## Structure

### Philosophy
* Modern JS (es6 (arrow, modules, array func...), webpack, babel)
* JS centric
* [if](https://hackernoon.com/rethinking-javascript-the-if-statement-b158a61cd6cb)
* pwa + front opti (fav, theme, metas, og, banner, responsive, ssl, svg)
* command-line deployment
* ut - ci - automated test
* no dependecies

### View
* src/components
* src/common
* public

### Model
* local storage
* session storage
* offline first (demo)
* easy to roll out

## Improvements
* better tests
* server-side verification
* server-side rendering
* add member id
* custom JSX
* custom Data-binding
* custom routing
[post](https://hackernoon.com/how-i-converted-my-react-app-to-vanillajs-and-whether-or-not-it-was-a-terrible-idea-4b14b1b2faff)

---

## Dev log

### Analysis and paper draft - 1h
I'm first working on a white paper, writing and drawing a rough representation of the model and its interactions, based on the stories.

#### Tools & stack
* Plain JavaScript + Babel (transpiling ES6 to ES5)
* Webpack (module bundler)
* NPM (package manager)
* ESLint (linting utility)
* Firebase (cloud solution)
* Atom (text editor)
* GitHub & GitKraken (code versioning)
* Circleci (running unit testing on PR)

*While benchmarking DB solutions, AWS or PouchDB seemed like good alternatives to `Firebase`. However, it offers great features (offline syncing, easy authentication, https, shared state) and a lower learning curve, in a very handy way.*

*`ESLint` allows a team to follow the same guidelines while writing code. It also reduces mistakes when coupled with a text editor such as Atom, that will trigger live warnings. I arbitrarily chose the `standard` mode but it could (should) be customized according to the team's preferences.*

### Project scaffolding - 1h
Project setup covers the following scope:
* Webpack configuration (ES6, HRM...)
* Node modules installation
* Writing custom NPM scripts
* GitHub repository & circleci setup
* ESLint setup
* Folder architecture (components-based) & documentation draft
* Cloud setup (CDN, DB) and dummy call to DB
* Dummy static files to test webpack configuration and circleci integration

*From my experience, that part is often underestimated but it will impact the project on the long run. However, for the sake of simplicity (prototyping), I didn't spend too much time on it.*

### Hosting
* s3
* certificate manager
* CloudFront
* route53
* S3 sdk

### QA
* test browsers

### last words
* challenging/fun
