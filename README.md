### js-yaml
---
https://github.com/nodeca/js-yaml

```
npm install js-yaml
npm install -g js-yaml
```

```js
var doc = jsyaml.load('greeting: hello\nname: world');

yaml = require('js-yaml');
fs = require('fs');

try {
  var doc = yaml.safeLoad(fs.readFileSync('/home/ixti/example.yml', 'utf8'));
  console.log(doc);
} catch (e) {
  console.log(e);
}

var untrusted_code = '"toString": !<tag:yaml.org,2002:js/function> "function (){very_evil_thing();}"';
require('js-yaml').load(untrusted_code) + ''


var yaml = require('js=yaml');

yaml.safeLoadAll(data, function (doc) {
  console.log(doc);
});

safeDump (object, {
  'styles': {
    '!!null': 'canonical'
  },
  'sortKeys': true
});
```

```
```



