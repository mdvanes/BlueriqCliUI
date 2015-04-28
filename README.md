# BlueriqCliUI

> CLI and text-adventure interface for Blueriq.


## Installation

* Install Blueriq 9.4.1 Java
* put UI/cli.stg in aquima.home/UI/mvc
* configure aquima.properties to have a theme cli that points to cli.stg.
* Node must be installed
* Clone this project and run ```nmp install``` in the dir with the package.json

Future versions will be installable through NPM, but will always require a configured and licensed Blueriq server.


## Usage

* start Blueriq server
* run: ```node index.js```
* type ```help```


## TODO

* consider renaming to BlueVermin
* views for different types of questions: domains, booleans etc.
* parametrize config.host/port/project etc.
* handle refresh/page submits (handle event is called with ajax POSTs: e.g.: http://localhost:8080/war/server/session/sessionId/api/subscription/subscriptionId/handleEvent ). For more info see REST API documentation at https://my.blueriq.com/display/BQ93/REST+API > SessionService
* release NPM package
* add screenshots to the readme
* refactor to be MVC? what is a backend MVC framework? Express? Sailsjs, KoaJs, HapiJs.
  Flatiron JS actually has a generator for CLI. Example app: https://github.com/vesln/todo
  But flatiron assumes you will run from the OS CLI and call it like: todo add bla, so no interactive console.
* serverside typescript? (problems: how to use test framework; maybe Node supports ES6 features natively, with harmony flag)
* compile to executable with e.g. EncloseJS http://enclosejs.com/ or is installation with NPM good enough?


## Changelog

* added logo (the origin of the logo is: http://www.chris.com/ascii/index.php?art=animals/rodents/mice)
* add grunt/jshint/lintspaces
* Removed model stub: load model from Blueriq Server (maintain the session)
* Display error when the server hasn't started yet
* Run start when the application starts
