# JavaScript

## Editor
- Use 2 spaces identation (no tabs)
- Use utf-8 charset
- Use LF (`\n`) for end of lines (see [`Wikipedia`](http://en.wikipedia.org/wiki/Newline))

This config is available in a [`.editorconfig`](.editorconfig)

## Strict mode
Always declare `'use strict';` at the top of your files.

if the file may be required by external code, bind it into a closure for exemple :
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
- Use english only.
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

# Licence
OpenDena coding-style is under the MIT licence. Please see 
[`LICENSE`](LICENSE)
