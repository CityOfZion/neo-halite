
# Neo Black Orc Plan
Neo-One Neo-Black Orchestration System Draft v1

# Build rough outline of Neo-Black Orchestration requirements
* Determine additional modules for control, if needed, and if rpc can run everything alone
  * Integrate RPC control module into Neo-Black
  * Integrate command line control module into Neo-Black (if needed)


# Build Presentation Framework (front end)

  Bring up fastest option first (Neo-Black Actual)
  * electron comes later as desktop integration
  * react
  * redux
  * webpack front end

## Screens for Neo-Black Presentation Framework (front end) (WIP)

This sections describes the control surface views within the front end.

  * Login
  * Configure Private Net
  * Configure Wallets
  * C&C Neotracker
  * Configure Application
  * C&C Neo-One (PRIORITY)
  * New neo-one Instance
  * Start/restart neo-one instance
  * Stop neo-one intance
  * View Running Instances
  * View Past Instances (logs too perhaps)
  * Restore Past Instances



# Control Surfaces (API)

At this time, it looks like most of the system control is done via command line and process management that is OS-specific.

Systems that we need to control:
 * Neo-One
  * Neo-tracker
  * @neo-one/client
  * @neo-one/smart-contract

* Neo-One-Playground
  * https://github.com/neo-one-suite/neo-one-playground

* Neo network RPC control via neo-tools RPC module

  These have been tested with neo-tools

  * https://github.com/neo-one-suite/neo-one/blob/ec89546f72b4ec12b499337434efeac4dae6d7a0/packages/neo-one-client-core/src/provider/JSONR


* grpc controls?
  * https://github.com/neo-one-suite/neo-one/blob/7781fc1ab09107d8301bade113538ddae761b3c7/packages/neo-one-server-grpc/proto/server.proto



# Build

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app) and fine-tuned to support Electron by [UVMetal](https://github.com/uvmetal).

## Notes

If you have problems with sqlite3 on Ubuntu 18 or similar, you may need to do the following:

```
npm install sqlite3 --build-from-source

```

## Available Scripts

In the project directory, you can run (I prefer to replace `npm` with `yarn`):

### `npm start`

Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br>
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.<br>
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.<br>
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br>
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (Webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.


### `yarn electron-dev`

Run a dev version packaged with Electron.

### `yarn electron-pack`

Package a distribution file with Electron and send it to the `./dist/` folder.

For example, to run stand-alone, do:

```
cd ./dist
./neoblack\ 0.1.0.AppImage
```

### `yarn electron-prepack`

Build react first, then package with Electron

### `yarn clean`

Delete the ``./dist/`` folder. This can grow quite large.


## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: https://facebook.github.io/create-react-app/docs/code-splitting

### Analyzing the Bundle Size

This section has moved here: https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size

### Making a Progressive Web App

This section has moved here: https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app

### Advanced Configuration

This section has moved here: https://facebook.github.io/create-react-app/docs/advanced-configuration

### Deployment

This section has moved here: https://facebook.github.io/create-react-app/docs/deployment

### `npm run build` fails to minify

This section has moved here: https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify
