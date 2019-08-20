# React Base Template

This is a base configuration to start React projects.

## Setting up 

`$ git clone url

`$ npm install

## Commands

### `npm start`

Runs the app in development mode.
Open http://localhost:1234 to view it in the browser.

Development mode comes with hot module reloading so the browser will automatically reload to changes with your code.

Any build errors will appear in the browser or console.

#### Linting

The project is linted through [AirBnB](https://github.com/airbnb/javascript).  Test files are ignored.

### `npm test`

Runs the tests for your application using [Jest](https://jestjs.io/docs/en/getting-started) and [Enzyme](https://airbnb.io/enzyme/) for unit and snapshot testing.

By default, it will look for any folder called `__tests__` within the `src/` directory.

### `npm run build`

Builds the application for production.

## Architecture

### `config/`

The `config/` directory holds all the Webpack configuration files.

- `webpack.config.js` contains all the general Webpack settings and common plugins to use across dev and build pipelines.
- `webpack.dev.js` contains development specific settings.
- `webpack.prod.js` contains production specific settings.

### `src/`

The `src/` directory contains all the source code for your application as well as any unit tests.  Jest will scan for any directory called `__tests__` for tests.

### `public/`

Holds any static files for your application and the `index.html` file the application uses.