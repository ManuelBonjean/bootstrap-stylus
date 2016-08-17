Bootstrap Stylus 3.3.7
======================

Port of the amazing [Bootstrap 3.3.7](https://github.com/twbs/bootstrap) to [Stylus 0.52.0](http://learnboost.github.com/stylus/).

## Installing

Via npm:

```bash
$ npm install --save https://github.com/ManuelBonjean/bootstrap-stylus
```
Example of requiring and using bootstrap middleware to create compile function to utilize in other frameworks.
```javascript
var bootstrap = require('bootstrap-stylus'),
	stylus    = require('stylus');

function compile(str) {
  return stylus(str)
	.use(bootstrap());
}
```

To import whole bootstrap in your stylus file:
```stylus
@import 'bootstrap-stylus/bootstrap/'
```

Alternatively to import individual components:
```stylus
@import 'bootstrap-stylus/bootstrap/variables'
@import 'bootstrap-stylus/bootstrap/mixins'
@import 'bootstrap-stylus/bootstrap/alerts'

```

## Copyright and license

Copyright 2013 Twitter, Inc under [the Apache 2.0 license](LICENSE).
