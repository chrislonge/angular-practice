angular-practice
================

Instructions on how to set up a full Angular development enviroment with Yeoman. I've also added instructions on how to set up a basic web server using NodeJS.

### Setting up Full Dev Env w/ Yeoman

You will need NodeJS, NPM, Yeoman, Grunt, and Bower

After you have installed Node.js and NPM run the following commands (remove "sudo" if you are on a windows computer):

`$ sudo npm install -g yo grunt-cli bower`

Make sure everything is installed as expected:

`$ yo --version && bower --version && grunt --version`

Install the Yeoman generator for AngularJS:

`$ sudo npm install -g generator-angular`

#### Generate An Angular App

1. Make directory & cd into it: `$ mkdir myAppName && cd myAppName`
  * Generate by running: `$ yo angular`
    * Optionally passing an app name: `$ yo angular [app-name]`
  * Answer Yeoman questions 

2. Install project dependencies: 
    `$ sudo npm install`

3. Start the server:
    `$ grunt serve`

### Setting up a Basic Web Server

1. Install connect and serve-static modules
  * `$ npm install connect serve-static`
2. Create server.js script and place it in your node_modules folder
  ```
  var connect = require('connect');
  var serveStatic = require('serve-static');
  connect().use(serveStatic(__dirname)).listen(5000);
  ```
  * __dirname is the directory you would like to serve
 
3. Run the script with NodeJS
  * `$ node server.js`
 
4. Open up browser to `http://localhost:5000/yourfile.html`
