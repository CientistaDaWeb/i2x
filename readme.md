# I2X-starter

> I2X challenge: [live demo](https://i2x-app.herokuapp.com/)

---


## Install

```sh
git clone https://github.com/vitormalencar/i2x
cd i2x
npm install
npm run build
npm start
```

> :exclamation: Use [Yarn](https://yarnpkg.com/) to install dependencies 3x faster than NPM!

## Features

* Offline Caching (via `serviceWorker`)
* SASS & Autoprefixer
* Asset Versioning (aka "cache-busting")
* ES2015 (ES6) and ES2016 (ES7) support
* Webpack Bundle Analysis (see [dashboard](#dashboard))
* Hot Module Replacement (HMR) for all files
* Preact's [Developer Tools](#preact-developer-tools)
* [Lighthouse](https://github.com/GoogleChrome/lighthouse) certified
  ![lightouse](docs/score.png)

## Development

### Commands

Any of the following commands can be run from the command line.

> If using [Yarn](https://yarnpkg.com/), all instances of `npm` can be replaced with `yarn`

#### build

```
$ npm run build
```

Compiles all files. Output is sent to the `dist` directory.

#### start

```
$ npm start
```

Runs your application (from the `dist` directory) in the browser.

#### watch

```
$ npm run dev
```

Like [`start`](#start), but will auto-compile & auto-reload the server after any file changes within the `src` directory.

### Dashboard

With [`webpack-dashboard`](https://github.com/FormidableLabs/webpack-dashboard), it's much easier to see what's happening inside your bundles. In addition to de-cluttering your `webpack-dev-server` log, you can quickly make sense of your bundles' `import`s and sizes.

![dashboard](docs/dev-dash.jpg)

The dashboard is meant to be interactive (scrollable). If you are having issues, please see the author's note:

> ***OS X Terminal.app users:*** Make sure that **View → Allow Mouse Reporting** is enabled, otherwise scrolling through logs and modules won't work. If your version of Terminal.app doesn't have this feature, you may want to check out an alternative such as [iTerm2](https://www.iterm2.com/index.html).

### Preact Developer Tools

You can inspect and modify the state of your Preact UI components at runtime using the [React Developer Tools](https://github.com/facebook/react-devtools) browser extension.

1. Install the [React Developer Tools](https://github.com/facebook/react-devtools) extension
2. [Import the `preact/devtools`](src/index.js#L21) module in your app
3. Reload and go to the 'React' tab in the browser's development tools

## License

MIT © [Vitor Alencar](https://vitormalencar.com)