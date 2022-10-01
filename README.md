# WeatherNavigator App
A weather application using the OpenWeatherMap API and GeoDB API with places autocomplete, along with React skills. <br/>
Jump to: [`React weather app final look.pic.jpg`](https://github.com/KrystalZhang612/WeatherNavigator-App/blob/newbranch/React%20weather%20app%20final%20look.pic.jpg)
# Developing tools: 
[Windows 10 Linux Ubuntu](https://ubuntu.com/tutorials/install-ubuntu-on-wsl2-on-windows-10#1-overview)<br/>
[Visual Studio IDE 2022](https://visualstudio.microsoft.com/vs/)<br/>
[NodeJS(node-v16.17.1-x64)](https://nodejs.org/ca/blog/release/v16.17.1/)<br/>
- [Method pushing Vscode from Linux system to Github branch](https://stackoverflow.com/questions/45891052/vs-code-how-to-use-github-with-existing-local-project):<br/>
In Vscode Terminal: <br/>
`git init .`<br/> 
`git config --global user.name <yourGitHubAccount>`<br/> 
`git config --global user.email <yourGitHubEmailAccount>`<br/> 
`git add .`<br/>
`git status`<br/> 
`git commit -m "COMMIT MESSAGE"`<br/> 
`git remote add origin https://github.com/<yourGitHubAccount>`<br/>
`git push -u origin master`<br/>
- Method replacing main branch with the new branch in Pull request:<br/>
Change New Branch in Github account `branches` section into Default Branch. <br/>

# Build 
[Prerequisites & Setups](https://github.com/KrystalZhang612/WeatherNavigator-App/blob/newbranch/README.md#prerequisites--setups)<br/>
[Method Running The Project(Locally)](https://github.com/KrystalZhang612/WeatherNavigator-App/blob/newbranch/README.md#method-running-the-projectlocally)<br/>
[Debugging&Troubleshooting](https://github.com/KrystalZhang612/WeatherNavigator-App/blob/newbranch/README.md#debuggingtroubleshooting)<br/> 
[Synchronous Developing Notes](https://github.com/KrystalZhang612/WeatherNavigator-App/blob/newbranch/README.md#synchronous-developing-notes)

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
Create a new folder under [src](https://github.com/KrystalZhang612/WeatherNavigator-App/tree/newbranch/src) named [components](https://github.com/KrystalZhang612/WeatherNavigator-App/tree/newbranch/src/components), create a new folder under components named [search](https://github.com/KrystalZhang612/WeatherNavigator-App/tree/newbranch/src/components/search), create a new file under search named [search.js](https://github.com/KrystalZhang612/WeatherNavigator-App/blob/newbranch/src/components/search/search.js).<br/>
In [search.js](htps://github.com/KrystalZhang612/WeatherNavigator-App/blob/newbranch/src/components/search/search.js):<br/>
Start by constructing a testing component:<br/>
```JavaScript 
const Search = () => {
return (‘Hello’)}
export default Search; 
```
Then import the component in [App.js](https://github.com/KrystalZhang612/WeatherNavigator-App/blob/newbranch/src/App.js):<br/>
```JavaScript 
import Search from ‘./components/search/search’; 
...
<Search />
```
Here, the localhost screen should print “Hello”.<br/>
Add a container:<br/>
In [App.js](https://github.com/KrystalZhang612/WeatherNavigator-App/blob/newbranch/src/App.js), set up the container’s widths and center margins:
```JavaScript 
.container {
  max-width : 1080px;
  margin: 20px auto;
}
```
Setting up text fonts and background color:<br/>
In [index.css](https://github.com/KrystalZhang612/WeatherNavigator-App/blob/newbranch/src/index.css):<br/>
```css
font-family: “Roboto”, Arial!important; ...
background-color: #d5d4d4
```
Now proceed to build our Search components. Back to [search.js](htps://github.com/KrystalZhang612/WeatherNavigator-App/blob/newbranch/src/components/search/search.js):<br/>
Import `useState` and `AsyncPaginate` to fetch data:
```JavaScript
import {useState} from “react”;
import {AsyncPaginate} from “react-select-async-paginate”;
```
Async paginate needs essential parameters:<br/>
A placeholder to prompt user input searching query:<br/>
```JavaScript 
Placeholder = “Search for a city”
```
To time out the data fetching:
```JavaScript 
debounceTimeout = {600}
```
Also a dynamic `onChange` to handle synchronous changes:
```JavaScript 
onChange = {handleOnChange}
```
To make the search parameters effective and visible, call it in [App.js](https://github.com/KrystalZhang612/WeatherNavigator-App/blob/newbranch/src/App.js):
```JavaScript
const handleOnSearchChange = (searchData) => { Console.log(searchData)}
...
<Search onSearchChange = {handleSearchChange} />
```
Refresh localhost, the searching placeholder with a query prompt should be visible.<br/>
Since we are loading properties through async paginate, we need to call `loadOptions` to fetch the certain APIs when retrieve the input values to implement the fetching method:<br/>






# Debugging&Troubleshooting
- Noticeable Setup Error: <br/>
`‘npm’ is not recognized as internal or external command, operable program or batch file `  warning occurs when trying to run the npm command. DEBUGGING: Go to [Node.JS](https://nodejs.org). Install `node-v16.17.1-x64` to Local Disk C: <br/>
Then in Vscode Terminal, install:<br/>
`npm i-react-select-async-paginat`<br/>
Ignore `high vulnarbilities` warnings.<br/>
Instead, do: `npm i-react-select-async-paginat --force` to add more protections. <br/>
- Possible Error When Activating React App: `Warning react-scripts: command not found`<br/>
DEBUGGING: install react-script globally instead: `npm install -g react-scripts` <br/>
- Stubborn Error `Access Denied` when removin @emotions fallbacks in node_modules inherited from npm package. DEBUGGING: [Access denied Win 10 Solution]( https://answers.microsoft.com/en-us/windows/forum/all/access-denied-windows-10/2a5429ee-dc93-4095-8058-a5ecfd2b69c9). 
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
