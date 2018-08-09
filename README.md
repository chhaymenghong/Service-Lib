## Project Overview
- This is a seed project for creating a new Angular 6 library with only service class. components/directives/pipes class should not be mixed within a library
with service class, normally we have to include the module for components/directives/pipes in all the modules that need them, whereas we only want
to include a module with service class once at the root module of the app.

- The project has two main entities. ```Service-App``` and ```Service-Lib``` under ```projects``` directory. ```Service-App```
should be used to document how to use ```Service-Lib``` library.

- Circle CI is used to automatically publish only ```Service-Lib```, the library and not the app, to npm registry. The publish
job is only run on successful merge to ```master``` branch. Any other projects that need to use this library can just install it
directly from npm registry.

- Don't forget to increment projects/service-lib/package.json to the appropriate version before the library is published to npm.

## Installation
- Install Node 10.8.0.
- Install Angular-Cli:  ```npm install -g @angular/cli```.
- Install dependencies: ```npm install```.

## Building/Running
- Consult ```package.json``` at the root of the project to learn more about all the development workflow scripts.

## Generate Angular models and services from Swagger 2.0 specification
- https://www.npmjs.com/package/ng-swagger-gen
