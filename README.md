# WeatherNavigator App
A weather application using the OpenWeatherMap API and GeoDB API with places autocomplete, along with React skills. <br/>
Jump to: [`React weather app final look.pic.jpg`](https://github.com/KrystalZhang612/WeatherNavigator-App/blob/newbranch/React%20weather%20app%20final%20look.pic.jpg)
# Developing tools: 
[Windows 10 Linux Ubuntu](https://ubuntu.com/tutorials/install-ubuntu-on-wsl2-on-windows-10#1-overview)<br/>
[Visual Studio IDE 2022](https://visualstudio.microsoft.com/vs/)<br/>
[NodeJS(node-v16.17.1-x64)](https://nodejs.org/ca/blog/release/v16.17.1/)<br/>

# Build 
Prerequisites & Setups<br/>
[Method Running The Project(Locally)](https://github.com/KrystalZhang612/WeatherNavigator-App/blob/newbranch/README.md#method-running-the-projectlocally)<br/>
[Debugging&Troubleshooting](https://github.com/KrystalZhang612/WeatherNavigator-App/blob/newbranch/README.md#debuggingtroubleshooting)<br/> 
[Synchronous Developing Notes]()

# Prerequisites & Setups
## ***Getting API Keys:***
To find open APIs, go to [GeoDB Cities](https://rapidapi.com/wirefreethought/api/geodb-cities/)<br/>
Sign up, and subscribe to the `GeoDB Cities API Test` -> `Endpoints` -> `Cities`<br/>
Then we have all code snippets and optional parameters to choose. <br/>
Go to [OpenWeather](https://openweathermap.org/): <br/>
Sign up. In My Account generated my unique API keys and services. <br/>
In `Linux Ubuntu Terminal`:<br/>
`npx create-react-app react-weather-app`<br/>
This will take a few minutes to install the React App packages, it is ready once terminal says:<br/>
`we suggest that you begin by typing:`<br/>
`cd react-weather-app`<br/>
`npm start`<br/>
`Happy hacking!`<br/>
Open the created folder in the local address with Vscode IDE.<br/>
## ***Setups: Creating the application and installing packages:***
In Vscode Terminal, install two essential prerequisite packages before starting:<br/>
`Npm i react-accessible-accordion`<br/>
## ***Activate React app:***
`Npm run start`<br/>
React app setups and activation work if we are redirected automatically by Node.JS to `localhost:3000` and message in Powershell terminal returns:<br/>
`Compiled successfully!`<br/>
`...`<br/>
`Webpack compiled successfully`<br/>
# Synchronous Developing Notes


# Debugging&Troubleshooting
- Noticeable Setup Error: <br/>
`‘npm’ is not recognized as internal or external command, operable program or batch file `  warning occurs when trying to run the npm command. DEBUGGING: Go to [Node.JS](https://nodejs.org). Install `node-v16.17.1-x64` to Local Disk C: <br/>
Then in Vscode Terminal, install:<br/>
`npm i-react-select-async-paginat`<br/>
Ignore `high vulnarbilities` warnings.<br/>
Instead, do: `npm i-react-select-async-paginat --force` to add more protections. <br/>
- Possible Error When Activating React App: `Warning react-scripts: command not found`<br/>
DEBUGGING: install react-script globally instead: `npm install -g react-scripts` <br/>
- 








# Method Running The Project(Locally)

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
