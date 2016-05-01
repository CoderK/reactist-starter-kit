## Reactist Starter-Kit

This project is composed of the following things.

React & Trnaspiler  

- React: [A JavaScript library for building user interfaces](https://facebook.github.io/react/)
- Webpack: [Module Bundler](https://webpack.github.io/)
- Babel: [The compiler for writing next generation JavaScript](https://babeljs.io/)

Flux Implements

- Redux: [Predictable state container for JavaScript apps](http://redux.js.org)

Test Framework

- Mocha: [Simple, flexible, fun javascript test framework for node.js](the browser http://mochajs.org)
- Karma: [Spectacular Test Runner for Javascript](https://karma-runner.github.io/)

Test Utilities

- Enzyme: [JavaScript Testing utilities for React](http://airbnb.io/enzyme/)

All build tasks is executed by npm. There is no reason. Just I have always wanted to develop without grunt or gulp.


### Directory Layout

```
.
├── coverage 	                          # coverage report
├── dev-server 	                   		  # webpack-dev-server's index.html
├── node_modules                          # npm third-party libraries and utilities
├── dist 	                              # build directory
├── src                                   # sample source code                 
├── test-helper                           # some files needed by karma
├── karma.conf.js                         # karma config file
├── package.json                          # npm build task and the list of 3rd party libraries and utilities
└── webpack.config.js                     # webpack configuration
```

### Getting Started

Just clone the repo and start hacking:

```shell
$ git clone https://github.com/CoderK/reactist-starter-kit.git my-app
$ cd my-app
$ npm install                   	# install dependencies
$ npm start                     	# compile and launch a webpack-dev-server
$ open localhost:8080				# open sample app in a browser
```

### How to build

```shell
$ npm run build  				# build development
$ npm run build:production 	# build product
```

This will create bundle.js into '/dist' directory.


### How to run webpack in watch mode

```shell
$ npm run build:watch
```

### How to run webpack-dev-server

```shell
$ npm start
```

### How to deploy

```shell
$ npm run deploy
```
This will create bundle.min.js into '/dist' directory with using '--optimize-minimize' of WebPack option.

### How to test

Run unit tests powered by Mocha and Karma with the following npm command:

```shell
$ npm test
```

When you execute above, Karma run all unit tests with phantomjs. 
If you want to test on browser environment, you can use this command.

```shell
$ npm run test-debug
```

It will run all '*-test.js' files in `__tests__` directory.

### How to get coverage report

You can get coverage report with the following npm command:

```shell
$ npm run coverage
```

A coverage report will be created at '/coverage'



 

