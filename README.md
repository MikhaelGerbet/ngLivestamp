# angular-livestamp

Angular directive to show an auto-updating timeago text to your timestamped HTML elements (using [Livestamp.js](https://mattbradley.github.io/livestampjs/) and [Moment.js](http://momentjs.com/))

Copyright (C) 2016, Mikhael GERBET <frollon.noir@gmail.com>.

[![Build Status](https://travis-ci.org/MikhaelGerbet/angular-livestamp.png?branch=master)](https://travis-ci.org/MikhaelGerbet/angular-livestamp)
[![Coverage Status](https://coveralls.io/repos/github/MikhaelGerbet/angular-livestamp/badge.svg?branch=master)](https://coveralls.io/github/MikhaelGerbet/angular-livestamp?branch=master)

## Usage

Get both livestamp.js, moment.js and angular-livestamp

- via npm: by running ``` $ npm install angular-livestamp ``` from your console
- or via Bower: by running ``` $ bower install angular-livestamp ``` from your console

Include both livestamp.js, moment.js and angular-livestamp.js in your application.

```html
<script src="bower_components/moment/min/moment.min.js"></script>
<script src="bower_components/livestampjs/livestamp.min.js"></script>
<script src="bower_components/angular-spinner/angular-spinner.js"></script>
```

Add the module `angularLivestamp` as a dependency to your app module:

```js
var myapp = angular.module('myapp', ['angularLivestamp']);
```

You can now start using the mg-livestamp directive to display an auto-updating timeago text.
For example :

```html
<span mg-livestamp="2016-06-09 22:21:00"></span>
```

You can also pass timestamp, for example:

```html
<span mg-livestamp="1465426421"></span>
```

### Example

See [online example on Plunker](http://plnkr.co/edit/BGLUYcylbIVJRz6ztbhf?p=preview).

## License

Released under the terms of MIT License.

## Contributing

1. Fork repo.
2. `npm install`
3. `bower install`
4. Make your changes, add your tests.
5. `grunt test`
6. `grunt build` once all tests are passing. Commit, push, PR.