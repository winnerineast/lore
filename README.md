# lore

[![Build Status][circle-image]][circle-url] [![Slack Status][slackin-image]][slackin-url]

![lore](https://cloud.githubusercontent.com/assets/5898306/13093056/654b5c76-d4c0-11e5-8968-643aae655030.png)


Convention driven framework for building front-end applications using React/Redux. Heavily opinionated and highly respectful. Built on React, Webpack, Redux and React-Router.


### Orientation

Lore's goal is to provide a framework that makes it easy to build React applications and is capable of supporting a 
mature real-world application. To understand how the framework makes it easier to get started with React, and what
problems it's trying to solve, please see [the intro video on the homepage](http://www.lorejs.org) or through 
[this direct link](https://www.youtube.com/watch?v=u3cK4fz1GNg).

If you're new to React, you may be interested in this video discussing 
[the challenges building a React application from scratch](http://www.lorejs.org/videos/building-your-first-react-app/) 
as additional context on how Lore reduces the learning curve for React development.

### Features

There are a lot of demands on front-end applications as they evolve to support the growing demands of the user base. 
Lore's goal is to build support for many of those common feature concerns into the architecture. Below is a list of UI
concerns Lore addresses or is planning to address, linked to their documentation page:

* [Data Structure](http://www.lorejs.org/features/foundation/data-structure/)
* [AJAX Abstration Tier](http://www.lorejs.org/architecture/ajax-abstraction/)
* [Filtering](http://www.lorejs.org/features/challenges/filtering/)
* [Pagination](http://www.lorejs.org/features/challenges/pagination/)
* [Infinite Scrolling](http://www.lorejs.org/features/challenges/infinite-scrolling/)
* [WebSockets (real-time)](http://www.lorejs.org/features/challenges/websockets/)
* [Visual Cues](http://www.lorejs.org/features/challenges/visual-cues/)
* [Optimistic Updates](http://www.lorejs.org/features/challenges/optimistic-updates/)
* [Dialogs](http://www.lorejs.org/features/challenges/dialogs/)
* [Wizards](http://www.lorejs.org/features/challenges/wizards/)
* [Error Handling](http://www.lorejs.org/features/challenges/error-handling/)
* [404 Pages](http://www.lorejs.org/features/challenges/404-pages/)


### Documentation

The documentation for Lore is hosted at http://www.lorejs.org.


### Tutorial

There is a [tutorial for learning Lore](http://www.lorejs.org/quickstart/) on the website. It covers:

* Creating a new application
* Prototyping with mock data
* Routing
* Fetching data from an API
* Launching dialogs
* Authentication (logging users in)
* Authorization (restricting what users see)
* Resolving breaking API changes
* Pagination
* Infinite Scrolling
* Filtering
* Normalization
* Publishing


### Discussion
If you have any questions, feel free to [create an issue](https://github.com/lore/lore/issues/new). If you'd rather discuss over chat, there is a [Lore Slack Team](https://lorejs.slack.com) which you can join [using this link][slackin-url].


### Near-term Focus

Since Lore is still in active development, I'm going to list the things that have immediate focus here.

1. [[done](https://github.com/lore/lore/pull/168)] Simplify ability to extend `lore-hook-connect` with new blueprints and mappings (v0.12.3)
2. [in-progress] Add Quickstart section to display new tweets at top of Feed ([branch](https://github.com/lore/www.lorejs.org/tree/add-websockets-to-quickstart), [dev site](http://master.lorejs.org/quickstart/optimistic/overview/))
3. [in-progress] Add Quickstart section to connect WebSockets for real-time behavior ([branch](https://github.com/lore/www.lorejs.org/tree/add-websockets-to-quickstart), [dev site](http://master.lorejs.org/quickstart/websockets/overview/))
4. [[done](https://github.com/lore/lore/commit/1861f379faad984326682df89a6f726f613872e8)] Update `lore` to load initializers _after_ hooks (v0.12.4)
5. [[done](https://github.com/lore/lore/pull/169)] Update all packages to ES6 syntax
6. [[partial](https://github.com/lore/lore/pull/169) (need to expose cjs folder)] Update all packages to supply a `module` export for tree-shaking
7. [[done](https://github.com/lore/lore/pull/172)] Break out form-related packages into their own repo called [lore-forms](https://github.com/lore/lore-forms)
8. [in-progress] Update connect blueprints to more easily support uses cases like getting all data and merging local data with paginated data
9. Replace references to `React.PropTypes` with `react-prop-types`
10. Replace references to `React.createClass` with `react-create-class` (or drop `createClass` completely)
11. Update Quickstart to focus on ESNext (ES6 as alternate syntax, ES5 support is being dropped)
12. Publish v0.13
13. Send out Newsletter


### Note about React Hot Reloading

Dan Abramov's [Hot Reloading with Time Travel](https://www.youtube.com/watch?v=xsSnOQynTHs) talk from React Europe 2015 demonstrated an incredible (and unique) value proposition for Redux and the functional programming concepts it uses as a foundation. That functionality has since been packaged into a library called [react-hot-loader](https://github.com/gaearon/react-hot-loader), which has gone through two major versions, with the beta version for v3 currently in development.

While there are tutorials that demonstrate how to obtain that functionality in React applications ([webpack tutorial](https://webpack.js.org/guides/hmr-react/), [react-hot-loader tutorial]()) the library itself [does not currently work with react-router](https://github.com/gaearon/react-hot-loader/issues/449), which is why it's not included as part of the development environment for Lore.

Once those issues are resolved, Lore will investigate including it as a default development behavior, similar to the way the Redux DevTools are included by default starting in `v0.12`.


### Thanks
* [React](https://github.com/facebook/react) for a brilliant componentization library for JavaScript.
* [Redux](https://github.com/reactjs/redux) for a simple and expressive React architecture.  
* [React Hot Loader](https://github.com/gaearon/react-hot-loader)/[React Transform](https://github.com/gaearon/react-transform-boilerplate) 
for making UI development a more fun and magical experience (even if it is [about to be sunset](https://medium.com/@dan_abramov/hot-reloading-in-react-1140438583bf)).
* [Sails](https://github.com/balderdashy/sails) for showing that a framework can be both strongly opinionated and highly respectful.
* [Lerna](https://github.com/lerna/lerna/) for providing a sane solution for managing a monorepo.
* [Storcery](http://storcery.io) for providing the environment, discussion and impetus that gave birth to Lore.
* [April Zero](http://aprilzero.com) for showing just how beautiful web apps can be.  Your creation continues to inspire.
* [Backbone](https://github.com/jashkenas/backbone) for a wonderfully well-thought-out interface for an API abstraction tier.
* [Redux-Auth-Wrapper](https://github.com/mjrussell/redux-auth-wrapper) for demonstrating a simple and expressive way to handle authentication and authorization concerns. 


[circle-url]: https://circleci.com/gh/lore/lore
[circle-image]: https://circleci.com/gh/lore/lore.svg?style=shield&circle-token=6ef9571387d0e08d802f6769026fcf91fc30459f
[slackin-image]: https://lorejs-slack.herokuapp.com/badge.svg
[slackin-url]: https://lorejs-slack.herokuapp.com
