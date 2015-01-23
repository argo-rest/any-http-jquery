# AnyHTTP adapter for jQuery

[AnyHTTP](https://github.com/argo-rest/any-http) adapter for the
[jQuery](http://jquery.com/) library.

## Usage

This adapter is implemented as an ES6 module which can be installed
with [jspm](https://jspm.io) and loaded via
[SystemJS](https://github.com/systemjs/systemjs) as follows:

``` javascript
import {Http} from 'github:argo-rest/any-http-jquery';

var httpClient = new Http;
httpClient.
  get('https://example.com').
  then(({body, headers}) => {
    console.log("body:", body);
    console.log("content-type:", headers['Content-Type']);
  });
```
