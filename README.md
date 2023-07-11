# Text Editor PWA (progressive web applications)
---
## Table of Contents
- [Text Editor PWA (progressive web applications)](#text-editor-pwa-progressive-web-applications)
  - [Table of Contents](#table-of-contents)
  - [General Information](#general-information)
  - [Utilized Technologies](#utilized-technologies)
  - [Installation](#installation)
    - [To perform a local installation, please follow these steps:](#to-perform-a-local-installation-please-follow-these-steps)
  - [Usage](#usage)
  - [Features](#features)
  - [Contact](#contact)
  - [License](#license)

---
## General Information 

We are challenged to create a browser-based text editor that meets the criteria for a Progressive Web Application (PWA). We utilized an existing application and implement methods for data storage and retrieval using an IndexedDB database. To simplify this process, we use the `idb` package, a lightweight wrapper for the IndexedDB API commonly employed by Google and Mozilla. The resulting text editor will demonstrate proficiency in the course concepts and feature offline functionality.
 
---
## Utilized Technologies

- [javaScript](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/What_is_JavaScript): A programming language implemented for web development and scripting purposes.
- [node.js v18.16.0](https://nodejs.org/en): A scalable server-side JavaScript runtime environment.
- [exspress v4.17.1](https://www.npmjs.com/package/express): A web application framework utilized to construct server-side applications.
- [concurrently v5.2.0](https://www.npmjs.com/package/concurrently): A package used for managing and executing JavaScript tasks concurrently.
- [code-mirror-themes v1.0.0](https://www.npmjs.com/package/code-mirror-themes): A collection of themes designed for the CodeMirror text editor.
- [@babel/core v7.15.0](https://www.npmjs.com/package/@babel/core): A compiler that transforms modern JavaScript code into backward-compatible versions.
- [@babel/plugin-transform-runtime v7.15.0](https://www.npmjs.com/package/@babel/plugin-transform-runtime): A Babel plugin that transforms code to utilize runtime features and dependencies.
- [@babel/preset-env v7.15.0](https://www.npmjs.com/package/@babel/preset-env): A Babel preset that automatically configures environment-specific language transformations.
- [@babel/runtime v7.15.3](https://www.npmjs.com/package/@babel/runtime): A Babel runtime library providing helper functions for transformed code.
- [babel-loader v8.2.2](https://www.npmjs.com/package/babel-loader): A Webpack loader used to transpile JavaScript code using Babel.
- [@babel/plugin-proposal-object-rest-spread v7.20.7](https://www.npmjs.com/package/@babel/plugin-proposal-object-rest-spread): A Babel plugin enabling object rest/spread syntax proposals in JavaScript.
- [css-loader v6.2.0](https://www.npmjs.com/package/css-loader): A Webpack loader used to import CSS files and resolve CSS dependencies.
- [html-webpack-plugin v5.3.2](https://www.npmjs.com/package/html-webpack-plugin): A Webpack plugin that automatically generates HTML files with bundled assets.
- [http-server 0.11.1](https://www.npmjs.com/package/http-server): A command-line utility for running a simple HTTP server to serve static files.
- [idb v6.1.2](https://www.npmjs.com/package/idb): IndexedDB, a client-side database utilized for storing structured data in web browsers.
- [style-loader v3.2.1](https://www.npmjs.com/package/style-loader): A Webpack loader used to inject CSS styles into the DOM at runtime.
- [webpack v5.51.1](https://webpack.js.org/): A module bundler employed for transforming and bundling assets in JavaScript applications.
- [webpack-cli v4.8.0](https://www.npmjs.com/package/webpack-cli): A command-line interface used for configuring and running webpack builds.
- [webpack-dev-server v4.0.0](https://www.npmjs.com/package/webpack-dev-server): A development server for webpack that provides live reloading and hot module replacement.
- [webpack-pwa-manifest v4.3.0](https://www.npmjs.com/package/webpack-pwa-manifest): A Webpack plugin that generates a Progressive Web App (PWA) manifest file.
- [workbox-webpack-plugin v6.2.4](https://www.npmjs.com/package/workbox-webpack-plugin): A Webpack plugin used for generating a service worker using Workbox.

---
## Installation
Deployed application can be accessed in the [Heroku](https://still-lowlands-67934-50fa4cd99f6e.herokuapp.com/) cloud platform.

### To perform a local installation, please follow these steps:

**Prerequisites**

- [node.js v18.16.0](https://nodejs.org/en/) - It is recommended to download `node.js v18.16.0` since this application has only been tested with that version. 
- [Google Chrome](https://www.google.com/) - Web browser developed by Google.

**Local Installation**

To use the `Text Editor PWA`, the user needs to complete the following steps: 

1. Clone the repository:
  - Go to the [Git-Hub](https://github.com/JonathanFadera/text_editor_pwa)
  - Clone the repository to your local computer.
2. Navigate to the Text Editor PWA directory:
  - Open a command line interface (e.g., Terminal).
  - Change directory to the Text Editor PWA repository location. Use the command `cd ~/...` and replace `...` with the path to the Text Editor PWA directory.
3. Initialize [node.js](https://nodejs.org/en) modules:
  - In the command line, while in the Text Editor PWA root directory, run the command `npm i`.
  - This command will install the required Node.js modules for the application to function.
4. Start the application:
  - In the command line, type `npm start` to bundle the static files and start the server.
5. Open application in the browser:
  - Open [Google Chrome](https://www.google.com/) browser to use the applicatin. 
  - Include the `localhost:3000` URL in a dedicated section of the browser.
  - The application should now be up and running.

These steps should guide you through the process of setting up and running the Text Editor PWA successfully.

---
## Usage
- To access the deployed version of the Text Editor PWA, visit the [Heroku](https://still-lowlands-67934-50fa4cd99f6e.herokuapp.com/) cloud platform.
- The Text Editor PWA provides a user-friendly experience, allowing users to freely type without limitations. The entered data is automatically saved to both the browser's local storage and indexedDB when the editor loses focus. This ensures seamless work resumption and secure data storage across sessions. Users can easily retrieve their saved data after reopening the app, enhancing the convenience of the Text Editor PWA.
- To install the Text Editor PWA as an application, simply click the "install" button displayed in the screenshot. This action will initiate the installation process on your device, creating a desktop icon for quick and easy access.

Installation Button:

![Installation Button](/assets/images/install-button.png)

Desktop Icon:

![Desktop Icon](/assets/images/desktop-icon.png)

---
## Features
* Uses IndexedDB to create an object store and includes both GET and PUT methods

* The application works without an internet connection

* Automatically saves content inside the text editor when the DOM window is unfocused

* Bundled with webpack

* Uses service worker with workbox that Caches static assets

* The application uses babel in order to use async / await

* Application have a generated `manifest.json` using the `WebpackPwaManifest` plug-in

* Can be installed as a Progressive Web Application

---
## Contact
-  [JonathanFadera](https://github.com/JonathanFadera)
    
---
## License
- This project is open source and available under the [MIT](./LICENSE)