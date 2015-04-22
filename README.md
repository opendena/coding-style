# JavaScript

## Editor
- Use 2 spaces indentation (no tabs)
- Use utf-8 charset
- Use LF (`\n`) for end of lines (see [`Wikipedia`](http://en.wikipedia.org/wiki/Newline))

This config is available in a [`.editorconfig`](.editorconfig)

## Linters
We use [`jshint`](http://jshint.com/) and [`eslint`](http://eslint.org/).

Make sur your code pass the both with [`.jshintrc`](.jshintrc) and [`.eslintrc`](.eslintrc).
There is many plugins to run those linter while saving on your favorite editor.

## Line length
Line length must be 80 characters or less.

## Strict mode
Always declare `'use strict';` at the top of your files.

If the file may be required by external code, bind it into a closure for example :
```javascript
// bad
'use strict';
…

// good
(function() {
  'use strict';
  …
})();
```

## Naming conventions
- Use English only.
- Use camelCase for objects, functions, instances.
  ```javascript
  // bad
  var MYUSER = {}
    , user_uuid = ''
  ;
  
  // good
  var myUser = {}
    , userUuid = ''
  ;
  ```
- Use PascalCase for constructors or classes
  ```javascript
  // bad
  var user = new userObject();
  
  // god
  var user = new UserObject();
  ```

## Literal syntax
```javascript
// bad
var item = new Object();

// good
var item = {};

// bad
var items = new Array();

// good
var items = [];
```

## Strings
Use single quotes `''` for strings.
```javascript
// bad
var name = "Bob";

// good
var name = 'Bob';
```

## Leading commas
```javascript
// bad
var user = {
  firstName: 'Robert',
  lastName: 'MARTIN',
  role: 'admin',
  createdAt: '2015-04-14'
}

// good
var user = {
  firstName: 'Robert'
  , lastName: 'MARTIN'
  , role: 'admin'
  , createdAt: '2015-04-14'
}
```

# License
OpenDena coding-style is under the MIT license. Please see 
[`LICENSE`](LICENSE)
