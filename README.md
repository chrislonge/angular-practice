angular-practice
================

Setting up an AngularJS app using Yeoman.

### Pre-requisites

You will need NodeJS, NPM, Yeoman, Grunt, and Bower

After you have installed Node.js and NPM run the following commands (remove "sudo" if you are on a windows computer):
```
sudo npm install -g grunt-cli
sudo npm install -g bower
sudo npm install -g yo
```
or `sudo npm install -g yo grunt-cli bower`

Make sure everything is installed as expected:
```
yo --version && bower --version && grunt --version
```
Install the Yeoman generator for AngularJS:
```
sudo npm install -g generator-angular
```
### Generate An Angular App

1. Make directory & cd into it: `mkdir myAppName && cd myAppName`
  * Generate by running: `yo angular`
    * Optionally passing an app name: `yo angular [app-name]`
  * Answer Yeoman questions 

2. Install project dependencies: 
    `sudo npm install`

3. Start the server:
    `grunt serve`
