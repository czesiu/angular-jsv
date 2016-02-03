# angular-jsv
JSV (JSON+CSV) httpParamSerializer for AngularJS

### Installing

```bash
    bower install angular-jsv
```

### Adding dependency to your project

When you are done downloading all the dependencies and project files the only remaining part is to add dependencies on the `JSV` AngularJS module:

```js
angular.module('myModule', ['JSV']);
```

### Usage

Pass `JsvHttpParamSerializer` as paramSerializer in your $http service call.

```js
// Simple GET request example:
$http({
  method: 'GET',
  url: '/someUrl',
  paramSerializer: 'JsvHttpParamSerializer'
}).then(function successCallback(response) {
    // this callback will be called asynchronously
    // when the response is available
  }, function errorCallback(response) {
    // called asynchronously if an error occurs
    // or server returns response with an error status.
  });
```